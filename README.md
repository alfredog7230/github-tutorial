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
13. Enter your cloud9 workspace and where it says bash on the bottom of the screen type ```ssh -T git@github.com```
14. If you did all these steps correctly then ```Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._``` should appear.
 

---
## Repository Setup



---
## Workflow & Commands



---
## Rolling Back Changes