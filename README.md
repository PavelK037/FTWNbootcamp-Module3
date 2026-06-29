# FTWNbootcamp-Module3
A sample project for the track practice activities in Module 03 of the TWN Bootcamp course.

## Setup git on the local machine

<details>
<summary> Some list of useful git commands </summary>
- instal git (done)
- configure git, set:<br>
    git config --global user.name=PavelK037 <br>
    git config --global user.email=pavel.kostylev@outlook.com
<br />
- setup ssh keys on the remote repo

## Command line instructions
- clone remote newly created project from Github or from GitLab repo 
<br>
git clone git@github.com:github.com/PavelK037/FTWNbootcamp-Module3 <br>
cd FTWNbootcamp-Module3 <br>
git swith -c main <br>
touch AnotherReadme.md <br>
git add AnotherReadme.md <br>
git commit -m "Added new file AnotherReadme.md" <br>
git push origin main <br>

- For push existing folder<br>
  git init --initial-branch=main <br>
  git remote add origin git@github.com:github.com/PavelK037/FTWNbootcamp-Module3 <br>
  git add .  <br>
  git commit -m "Initial commit" <br>
  git push -u origin main <br>
 " -u, --set-upstream
           For every branch that is up to date or successfully pushed, add upstream (tracking) reference, used by argument-less git-pull(1) and other commands. For more
           information, see branch.<name>.merge in git-config(1)."
  <br />
  **the option -u, or --set-upstream use to push localy created branch to the remote repo.**
   <br />
  </details>...
  
