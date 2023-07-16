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


