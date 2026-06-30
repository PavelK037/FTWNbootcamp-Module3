# FTWNbootcamp-Module3

A sample project for the track practice activities in Module 03 of the TWN Bootcamp course.

## Command Line Instructions

Below is a reference list of useful Git commands for setting up and managing this repository.

### 1. Initial Git Configuration
Set up your global user identity on your local machine before committing code:

```bash
# Configure global user name and email
git config --global user.name "PavelK037"
git config --global user.email "pavel.kostylev@outlook.com"
```

### 2. Scenario A: Cloning a New Remote Repository
Use this workflow if you have already created a blank repository on GitHub or GitLab and want to bring it down to your local development machine.
```bash
# Step 1: Clone the remote repository to your local machine via SSH
git clone git@github.com:PavelK037/FTWNbootcamp-Module3.git

# Step 2: Navigate into the newly cloned project directory
cd FTWNbootcamp-Module3

# Step 3: Explicitly create and switch to the 'main' branch
git switch -c main

# Step 4: Create a new test file
touch AnotherReadme.md

# Step 5: Stage the newly created file for tracking
git add AnotherReadme.md

# Step 6: Commit your staged changes with a descriptive message
git commit -m "Added new file AnotherReadme.md"

# Step 7: Push the committed local changes to the remote repository
git push origin main
```
### 3. Scenario B: Pushing an Existing Local Folder to a Remote Repository
Use this workflow if you have an existing directory of code on your local computer that you want to transform into a Git repository and push up to a newly created, empty remote repository.
```bash
# Step 1: Initialize Git tracking inside the root of your existing project folder
git init --initial-branch=main

# Step 2: Link your local repository to the remote target endpoint on GitHub
git remote add origin git@github.com:PavelK037/FTWNbootcamp-Module3.git

# Step 3: Stage all existing files in the directory for tracking
git add .

# Step 4: Capture your initial state snapshot with a commit
git commit -m "Initial commit"

# Step 5: Push local commits up to the remote main branch and track upstream
git push -u origin main
```
### 4. Technical Concepts & Deep Dives
Understanding the `-u` or `--set-upstream` Flag
When initializing a repository locally and pushing it for the first time, using `git push -u origin main` is a critical optimization pattern.

- The Mechanics: The `-u` flag creates an upstream tracking link between your local branch (main) and its counterpart on the remote server (`origin/main`).

- The Benefit: Once this link is configured, you no longer need to write verbose target names when interacting with the server. Git automatically populates the defaults from your configuration file (`branch.main.merge`),

Complete Command
`git push origin main`
`git pull origin main`
Shorthand Equivalent (After -u) 
`git push`
`git pull`

