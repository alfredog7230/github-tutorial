# GitHub Tutorial

_by Alfredo Gutierrez_

---
## Git vs. GitHub

_Git_: Is where you keep "snapshots" of your code but does not require **Github**.   
**GitHub**: Is where you store the code that you took snapshots of, however **Github** does require _Git_.

---
## Initial Setup
To set you up you will have to follow these directions:
1. Go to [github.com](github.com).
2. Create an accout on github.
3. After you finish creating your account you then go to the top right corner of your page and press on your profile icon.
4. Click on settings.
5. On the left side bar you should see a title that says SSH and GPG keys.
6. After that click New SSH key and name it "cloud9".
7. Go to [cloud9](c9.io).   
(If you have a cloud9 go to step 9 if you don't have a cloud9 account move to step 8)
8. Create a cloud9 account and make a new workspace.
9. Before you enter your workspace click on the gear icon on the top right of the page.
10. When you are there click the SSH keys.
11. After that go to github and copy the _2nd_ SSH key from github(should start with ssh-rsa).
12. Then paste to cloud9.
13. Enter your cloud9 workspace and where it says bash on the bottom of the screen type `ssh -T git@github.com`
14. If you did all these steps correctly then ```Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._``` should appear.
 
---
## Repository Setup

The way to set up a repository (repo for short) is simpler that the initial setup, just follow these next few steps to setup a repo.   
First off you need to open your [cloud9](c9.io) and your [github](github.com) and log in to both.   
Once you are logged on, go to your github account, press the "+" on your top right corner of your screen, and click "new repository".   
After that name the repo and create the new repository.   
Once you clicked "create repository", look for "quick setup" and make sure **SSH** is highlighted next to the url _not_ **_HTTPS_**.   
Then look for the subtitle that says "…or push an existing repository from the command line" and press the clipboard button that copies the command line that looks like this:  
```bash
git remote add origin https://github.com/alfredog7230/practice-repo.git
git push -u origin master
```   
After that, go to your cloud9 and go to your bash and create a new directory and name it **_EXACTLY_** how you named the repo.  
Then move into that directory and in bash paste what you copied into bash paste where it says:   
```bash
yourusername:~/workspace/yourrepo $ 
```
Ta-da you have copleted the Repository Setup!

---
## Workflow & Commands

In this part of the tutorial I am going to show you some key commands in git and the workflow.   
If you couldn't do the repository setup because you didn't know som code here is some code that will help you with the repo setup.   
`mkdir ` is used to make a directory.  
`cd` is used to move from file to file all you have to do is add the file you want to go to after the cd.   
`git` should go after every command you are writing except for a few.  
These next few commands are for more advanced coders.   
`git touch` is used to make a file inside a directory.
`git add` is used to add the changes you did to a file.
`git commit -m ""`is used after `git add` and is used yo write a "note" of what you currently did to the file. You would write the "note" in the quotation marks.   
`git push` is used to push everything that you changed to the repository that you just changed.
---
## Rolling Back Changes

Rolling Back Changes are very usedful when creating something in yuor file.
* `git checkout -- filename`
   * What this does is that whaever you had on a file before you edited it, the code will file will change back to the way you had it.
* `git reset HEAD filename`
    * What this does is that when you use `git add` and you didn't meant to you can use this to redo/undo what you just did.
* `git reset --soft HEAD~1`
    * Is used after you didn't meant to commit a file and you want to undo a commit you can simply use the code above to undo it.
* `git reset HEAD~1`
    * This is used when you want to undo a commit and add at the same time.
* `git reset --hard HEAD~1`
    * This command line is used to undo a commit, an add, and also the edits you did to a file. (Isn't that cool)