# gitsubmodule1

https://dev.to/serhatteker/changing-git-submodule-repository-to-other-url-branch-356p
</br>
<br/>
https://linuxhint.com/change-an-existing-submodules-branch/

<br/>
<br/>


**For Error Fix**
git submodule deinit -f src/JTA.Web/Vue <br/>
git rm -f src/JTA.Web/Vue <br/>
rm -rf .git/modules/src/JTA.Web/Vue <br/>
<br/>
# Before Build Commands
git submodule init ---> For origin Commit <br/>
git submodule update---> For Head Commit <br/>
# How to add submodule to Project
git submodule add -b feature/develop_DevOps http://odsgitlab1.odsdai.netdai.com/devops-offshore/daily-shift-report.git src/JTA.Web/Vue


# How to change the submodule for Repo

Step 1: Move to Local Main Repository <br/>

Step 2: Navigate to Submodule <br/>

Step 3: Check Submodule’s Branch <br/>
**git branch**
<br/>
Step 4: Change Submodule’s Branch <br/>
**git checkout master**
<br/>
Step 5: Move Back to Parent Repository
**cd ..**
<br/>
<br/> Step 6: Use git submodule update --remote
<br/> Step 7: Add Changes to Git Index

<br/> Step 8: Commit Changes

<br/>
# List the details in .gitmodules file
This command lists all the submodules present in the current repository with their paths, URL location and the branch which it is mapped in the repository. <br/>
  **git config --file=.gitmodules -l **

# Sync and update the Submodule
$  git submodule sync <br/>
$  git submodule update --init --recursive --remote </br>

