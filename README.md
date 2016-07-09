# GitStepsForWindows
Step by step to set up git in windows

Steps for adding your local Project to remote Github repository.

1. Crate your new repository  without any README.md or license file on your github account (ex:( https://github.com/raja0612/Java8Features.git)
2.Download abd Install git scm on your windows machine.(https://git-scm.com/download/win)
3. On your local machine, go to project workspace directory (ex: C:\Users\RAJASHEKHAR\workspace\jpa\Java8Features)
4.Initialize git repository (ex : git init)
5. add README.md  , .ignore files ( ex: touch README.md , touch .ignore  , these two commands will create those files)
6. add project description on README.md ( ex : vim README.md then enter "i" write text an then enter esc + :x)
7. add any files which you dont want to push remote repo  on .ignore file, same like vim .ignore then press i then start typing \bin ,\.classpath \.settings \.project \target and then esc :x 
8. add files which you want to push to remote repo 
  
    git add src
    git add README.md
    git add .ignore
    
    
9. git status (you will see all above files to be committees message)


10 . git commit -m "Message here"

11. add remote repo ( git remote add origin https://github.com/raja0612/Java8Features.git)

12. push changes to remote repo ( git push -u origin master)

13.next time onwards just git push 


----------------------------------------------------------------------------------------------------------


Steps for cloning and push local changes to remote repository.

1. Create Repository on your GitHub Account with readme file.

2. On your windows machine, Create Directory of your own to clone the repository.
  command: mkdir GitTutorial.

3.Change Directory to newly created directory on your windows machine: 
 command: cd GitTutorial:

4:Just make sure confirm , it's empty directory: (command: dir or ls : no files)

5.clone the git repository:

  command: git clone https://github.com/raja0612/GitStepsForWindows.git 

6. Now see list of files : mkdir or ls 
  you will see README.md

7. Create your own files to commit
   mkdir steps.txt.

8. now see the git status 

   command: git status

  you will observe untracked files in red color. (in my case Steps.txt)

9. add your local files to git
   command: git add steps.text ( To add all files git add -A)

10.   now see the git status:
  command: git status

now you will obeserve "Changes to committeed" in green color
  new file: Steps.txt

11. Commit to Git

  command: git commit -m "added steps.txt"

12. The files still in your local machine it means not sync up with your git hub account

   command:  git push

 you will observe on your console like below

Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 660 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/raja0612/GitStepsForWindows.git
   7c8f11e..bd0f494  master -> master




-----------------------------------------------------------------------------------------------------------------------------------------


 13. To get other team developers changes.

command: git pull


14: if you commit the chnages wihout message , esc + :wq to exit from screen

