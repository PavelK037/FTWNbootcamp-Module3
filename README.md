# FTWNbootcamp-Module3
A sample project for the track practice activities in Module 03 of the TWN Bootcamp course.

## Setup git on the local machine

- instal git (done)
- configure git, set:<br>
    git config --global user.name=PavelK037 <br>
    git config --global user.email=pavel.kostylev@outlook.com
<br>
- setup ssh keys on the remote repo
  
- clone remote newly created project from Github or from GitLab repo 
<br>
git clone git@github.com:github.com/PavelK037/FTWNbootcamp-Module3
cd FTWNbootcamp-Module3
git swith -c main
touch AnotherReadme.md
git add AnotherReadme.md
git commit -m "Added new file AnotherReadme.md"
git push origin main

- For push existing folder<br>
  git init --initial-branch=main
  git remote add origin git@github.com:github.com/PavelK037/FTWNbootcamp-Module3
  git add .
  git commit -m "Initial commit"
  git push -u origin main
 " -u, --set-upstream
           For every branch that is up to date or successfully pushed, add upstream (tracking) reference, used by argument-less git-pull(1) and other commands. For more
           information, see branch.<name>.merge in git-config(1)."
    ...
