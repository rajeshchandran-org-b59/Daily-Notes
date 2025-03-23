How we develop code locally ? Where do we publish it ?

GIT: Client based verison control system installed on computer or server

GitHub / GitLab / BitBucket: Centralized Version Control System

Git Flow
Computer to GitHub Authentication

If you're using Windows:
    1) GITBASH ( Install GitBash, this offers Git Client and terminal )
       > Click on windows button, click Git Bash and this opens the terminal for you.
    2) VS Code
        > Download and install it, once it's installed, just click on VSCode to open.

If you're using MacBook / Linux:
    1) Just install git ( Open your terminal : "$ brew install git" )
    2) Install VSCode for Mac

Once you install the VSCode, make sure to enable the "AUTO SAVE Option" on FILE and this saves all changes automatically.

GitHub Action is the CI/CD Framework which can learnt for free on GitHub, if your repositories are under an ORG and they are free.

Understand these terms:
    $ git clone repoName : This means downloading the whole repo to your local ( If the repo is public , it won't challenges with userName and password )
    $ git push : Once you made a clone, if you made some changes, we publish those changes back to the central repo 
    $ git pull : If there are some changes on the git repo, to download those changes, we use "git pull" 
    $ git commit -m "Standard Msg" : This is to give some message to the changes that you make 

# Wheneven want to push your changes, here are the steps to be followed 

    1) git add fileName-that's-changes or simply "git add ." this includes all the files in your directory
    2) git commit -m "EXP-APP-7: Updated the session-14 file"
    3) git push

Git HUB Uses PAT for authentication ( PAT: Personal Access Token )

If the repo is public:  
    1) You can clone the code without the need of credentails 
    2) If you want to push the code to the repo, you need to prove that repo is owned by you, by filling your credentials 

If the repo is private:  
    1) You can clone the code but need credentails 
    2) If you want to push the code to the repo, you need to prove that repo is owned by you, by filling your credentials 

VSCode Command To Open a Folder In VSCODE:
    $ code folderName

> Later: Code Review, Branching Strategy, Pull Reqeust

One time work:
    1) Singup github and create a org and repo's as needed under this 
    2) Clone the needed repo to batch59/ using git clone repoName 

Continuous Work:
    1) Develop locally 
    2) Publish the changes to gitHub 
    3) Pull the changes on server as needed 
    4) Test them as needed
