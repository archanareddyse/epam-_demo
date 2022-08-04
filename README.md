# epam-_demo
epam_demo
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Git Bash
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
$ git init
we observe two changes after this command 
1.it will create .git folder in the working directory
2. and it will as master branch
How to configure username and email for git
$ git config --global   user.name "archanareddyse"
$ git config --global   user.email  “archanareddycse@gmail.com”
$ git config –global  --list
Crete the file by file1,file 2
$ cat file1 and $ file2
Types of files 
Untracked files –can be seen by git status command which shows in red color
Staged files --- files can be can be stagged by git add command
Committed files --- by this command files are stored in local repository
$ git status
$ git add filename [for single file]
$ git add .[for more than files]
$ git commit -m “message for commit”
$ git log [shows us all committed messages]
or
$ git log --oneline
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
restore the files after stagging area
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Now create more files and check the status
Now add the files to stagging area by $ git add.
If you want to restore the files from the stagging area which are not committed the command is 
$ git restore –staged file2
$ git reset file2
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
If you want to restore the files which are  committed 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
$ git revert [commit id]
After revert command a file will displayed type message you to type to ignore the commit
:wq
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
How will see how push to local repository to git hub
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Create the github account 
Now create the new repository
Click on code will to get http link copy that and paste in git bash
$ git add .
$ git status 
$ git commit -m "message"
paste the copied url here 
$ git remote add origin url path
$ git remote -v
$ git push -u origin master
will be seeing all files are copied into it
go to github and refresh it will be seeing all files from local
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Branching Concepts:- when one or more persons are working on same project we use branching concept
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
We create file f1 in master and commit it as “a” commit
Create another file by f2 and commit as f2
Check log by $git log –oneline , we can see “a & b” commit
Now we create branch as archana 
$git branch <branch name>
We can see how many branches are present by 
$ git branch {* shows in which branch are in}
To get into branch we go for
$git checkout <branch name>
Now create some files in archana branch as files t1 and commit as “c”
Now will add few more files and change in file1 will see changes
$ git remote add origin copy the link of github repository
Now check the log history we get all master branch and archana branch commit there
Commit -a,b are from master
              -c,d are from archana
Now check out to master branch and create the another file f3 and commit as “e”
Now check the log we see only commits of master branch only
Git merge concept
For merging we must be master branch
$git merge archana
A pop window will be opend ->:q
Now check the log where will get all sequence of commits a,b,c,d,e and new commit a head
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

