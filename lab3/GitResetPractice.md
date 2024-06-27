## Steps: 
I first created a branch called  git-reset-practice. Then I created a single file *file.txt* in that branch. 
I created three commits called “Commit 1”, “Commit 2” and “Commit 3”.  In each commit file.txt contained text “version <commit_number>”. 
I logged all the commits with ```git log```

<img width="543" alt="Screen Shot 2023-06-26 at 15 38 26" src="https://github.com/FK12344321/labs/assets/69464701/c70df129-21a2-4866-9c31-3dfcf994d3da">

After that I entered ```git reset --soft 657133cdfb56e9dda0a35f2a562fa40f8c0d6b64```. I logged the commits again and saw that *HEAD* now was at commit two, but file.txt contained “version 3” and ```git status``` showed that changes of the third commit were also in the Index area.

<img width="548" alt="Screen Shot 2023-06-26 at 15 38 51" src="https://github.com/FK12344321/labs/assets/69464701/64efce07-78e3-4a85-a731-ad99ccbda79d">

I made a new commit “Commit 3” and returned to the initial state. 

After I did ```git reset --mixed HEAD~1``` and found out that the content of the file remained the same (*HEAD* was at commit 2)

<img width="385" alt="Screen Shot 2023-06-26 at 15 40 13" src="https://github.com/FK12344321/labs/assets/69464701/a000014b-6383-44f7-a405-b3313e6840eb">

but ```git status``` showed that the modification of the file was not staged

<img width="523" alt="Screen Shot 2023-06-26 at 15 41 04" src="https://github.com/FK12344321/labs/assets/69464701/5844370c-5214-4252-aa3c-8417b5c78615">

I added it to the stage area with ```git add file.txt``` and committed it and returned to the initial state again.

Finally, I did ```git reset --hard HEAD~1``` and saw that the working area was reset and the content of the file satisfied the second commit “version 2” and that the stage area was empty. In such a way I lost the content of the third commit. 

<img width="390" alt="Screen Shot 2023-06-26 at 15 41 32" src="https://github.com/FK12344321/labs/assets/69464701/6c813613-7a01-489c-a666-7fc6210a5dd6">


## Conclusion 
```git reset --soft <arg>``` just returns *HEAD* to the commit given as the argument and puts changes from the working area to the staged area. Better to use if you need to refactor your commit history return *HEAD* to some commit in history and make all the new commits from that commit. So the commit tree is more understandable and satisfies some logic of development. 

```git reset --soft <arg>``` leaves the working area as it is, but stage are gets empty and *HEAD* also gets returned to the arg commit. Can be in a similar way as soft, but also can be helpful if you want to reset the stage area. For example, if you accidentally added some redundant file 

```git reset --soft <arg>``` completely resets the working area and stage area, so the changes made after the argument commit get lost. If you made some unnecessary changes and want to return to some older commit, retract all the commits after that. 
