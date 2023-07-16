## Github Actions 
I just created a file ```github/workflows/github-actions-demo.yml```, copied the required content there and made a commit. After that I found a running pipeline in the Actions tab of the repository. All the jibs ran successfully 

<img width="734" alt="Screen Shot 2023-07-16 at 14 59 02" src="https://github.com/FK12344321/labs/assets/69464701/91912995-7d70-4ee9-b6db-472350a1b732">

After taht I committed a file called some_changes.txt to the root folder. This time The job that lists the files in the repo also showed the newly created file. I also decided to change pipeline a little bit and trigger some errors. In the step listing the content of the workspace folder I addred an unexisting folder , so the command looked like that ```ls ${{ github.workspace }}/folder```

The job failed with the following message

```
ls: cannot access '/home/runner/work/labs/labs/folder': No such file or directory
5
Error: Process completed with exit code 2.
```

## Extra task 
After that I edited the parameters of the ```on``` property and it looked ion the following way: 

```
on: 
  push: 
  workflow_dispatch:
```

But for some reason I was not able to trigger the run manually in the ```Actions``` tab. It turned out that it worked only if I push it to the ```main``` branch. I did that and finally was able to click the button ```Run workflow``` to trigger it.  

Then I added a new step to the job:

```
- name: Info about the system
        run: |
          echo "OS: ${{ runner.os }}"
          echo "CPU Cores: $(nproc)"
          echo "Memory: $(free -h)"
          echo "Operating System: $(uname -a)"
```

I printed out the info about the hardware (RAM and CPU), about the runner, and about the OS. Here is the output: 

<img width="1054" alt="Screen Shot 2023-07-16 at 20 27 26" src="https://github.com/FK12344321/labs/assets/69464701/f26634db-922d-4c71-940d-8cff802aebc4">
