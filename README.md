# IntroToGit
Repository to use for Git/GitHub practice


## Install git

Follow the instructions found here:

**MAC**

https://www.atlassian.com/git/tutorials/install-git#mac-os-x​

**Windows**

https://www.atlassian.com/git/tutorials/install-git#windows


## Instructions

1. **Fork** the upstream repo: https://github.com/minimester/IntroToGit to your account
2. **Clone** your forked repo to local computer (Don't forget to `cd` into your project folder!)
3. Setup your **remote** environment by establishing an upstream
4. Create and **checkout** a branch
5. Add your name to names.txt (Don't forget Paul's adoration for cuddly puppies!)
6. **Commit and push** changes to your repo
7. Create a **pull request** to upstream

**ALWAYS PUSH TO ORIGIN, _NEVER_ UPSTREAM**


## Reference
### Common Terms
| Term     | Definition |
|----------|------------|
| **Repository ("Repo")** | The database that stores the files | 
| **Working Directory** | Your local directory of files |
| **Revision** | The version that a specific files is on |
| **Branch** | A separate copy of the code, where changes can be made independently from the main "trunk" |
| **Fork** | A copy of a repository | 
| **Upstream** | Typically the repo that you forked from |
| **Pull request ("PR")** | A request to merge changes from one branch to another. Can be between branches across different forks of a repo |


### Basic Commands
| Command      | Usage | Example |
|--------------|-------|---------|
| **`git clone <repo_url>`**| Clone a repository into a new local directory | `git clone https://github.com/minimester/IntroToGit.git`|
| **`git remote [-v add]`** | Your remote environment, listing out references to online repositories. `-v` lists the reference name and corresponding link to the repository. `add <name> <repo_url>` adds a new reference (i.e. upsream or origin) to an online repository | `git remote -v add upstream https://github.com/minimester/IntroToGit.git` |
| **`git checkout [-b] <branch>`** | Switches to another branch on your local working copy. Adding the `-b` flag will create the branch if it doesn't exist and switch inside it | `git checkout -b myNewBranch` |
| **`git status`** | Shows the working tree status (files with changes, files ready for commit, etc.) | `git status` |
| **`git pull <reference> <branch>`** | Fetch from reference of online repo (usually "upstream") and integrate with local working directory | `git pull upstream master` |
| **`git add <file_name>`** | Adds a change in the working directory to the staging area | `git add names.txt` |
| **`git commit –m "<message>"`** | Record changes to a repo | `git commit -m "Added name"` |
| **`git push <reference> <branch>`** | Sends commits (code changes) to repo referenced (usually "origin") | `git push origin myNewBranch` |
