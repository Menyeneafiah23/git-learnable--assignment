# git-learnable--assignment

Explain Version control

Version control, also known as source control, is the practice of tracking and managing changes to software code. Version control systems are software tools that help software teams manage changes to source code over time. As development environments have accelerated, version control systems help software teams work faster and smarter. They are especially useful for DevOps teams since they help them to reduce development time and increase successful deployments. Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

Explain difference between git and github

Git: Git is a distributed version control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows. 

GitHub: GitHub is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features. 

List 3 other github alternatives

SourceForge
GitLab
Bitbucket

Explain the difference between git fetch an git pull?

git pull

git pull is used to fetch changes from a remote repository and integrate them into your current branch.
It automatically merges the fetched changes into your current branch.
It is essentially a combination of git fetch followed by git merge.

git fetch

git fetch is used to retrieve changes from a remote repository without integrating them into your current branch.
It updates your remote tracking branches (e.g., origin/master) to reflect the changes in the remote repository.
It does not modify your working directory or your current branch.
After fetching, you can review the changes and decide how to integrate them into your local repository using commands like git merge or git rebase.

Explain in simple terms git rebase and the command for it

Git rebase can integrate the changes from one branch to another by overcoming the problems that we might have faced while using the git merge command. The changes we will do will be recorded in the form of logs which are useful to go through if any mistakes happen.


Git Rebase Commands
The following are the most used Git rebase commands:

git rebase master: The command “git rebase master” can be used to make all modifications found in your master branch part of your current branch.

git rebase –continue: When we are rebasing the branches we will face some conflicts and issues then we need to resolve the issue. After resolving the issue we again continue the rebasing processes for that we use “git rebase –continue”.

git rebase –abort: “Git rebase –abort” command cancels a rebase that is currently underway and restores the branch to its initial state.

git rebase –skip: When rebasing the branches we might face some unresolved conflicts to skip the particular encounters we will use  “git rebase –skip”. Skipping the commit is not good practice it will damage your codebase.

git rebase -I HEAD~3: With the help of this command, you can interactively rebase the most recent three commits onto the active branch. You can choose which commits to rebase, alter commit messages, and squash or divide commits in the interactive editor that is opened.

Explain in simple terms git cherry-pick and the command for it 

cherry-pick refers to the process of selecting specific commits from one branch and applying them to another branch.


Command for it : 
To cherry-pick a single commit onto the current branch, use the following command:

git cherry-pick <commit-hash>

Cherry-Picking Multiple Commits:
You can cherry-pick multiple commits in a single command by specifying their commit hashes:

git cherry-pick <commit-hash-1> <commit-hash-2>

Cherry-Picking a Range of Commits:
If you want to cherry-pick a range of commits, you can use the following syntax:

git cherry-pick <start-commit-hash>^..<end-commit-hash>


