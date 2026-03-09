# wmwe-ssm-gitcontrols
This repository is meant to help students practice using Git and Github

# Git Workflow Guide

You will learn how to:

-   Clone a repository
-   Create a new branch
-   Add a new file
-   Commit your changes
-   Push your branch
-   Merge your branch

------------------------------------------------------------------------

# 1. Clone the Repository

First, download the repository to your local machine.

``` bash
git clone <repository-url>
```

Example:

``` bash
git clone https://github.com/anushap6571/wmwe-ssm-gitcontrols.git
```

Move into the project directory:

``` bash
cd wmwe-ssm-gitcontrols
```

------------------------------------------------------------------------

# 2. Create a New Branch

Create a branch for your changes

``` bash
git checkout -b feat/<feature name>
```

Example:

``` bash
git checkout -b add-readme
```

This creates a new branch AND switches you to it. If a branch already exists and you 
would like to go to it, 

``` bash
git checkout feat/<feature name>
```

------------------------------------------------------------------------

# 3. Add a New File

Create a new file in the project

Example:

``` bash
touch example.txt
```

Add some content to the file.

    Hello Git!

------------------------------------------------------------------------

# What is a `.gitignore` File?

A `.gitignore` file tells Git **which files or folders it should ignore and not track**.

This is useful for files that:
- are automatically generated
- contain sensitive information
- are not needed in the repository

Common examples include:
- dependency folders
- build files
- environment variables
- system files

------------------------------------------------------------------------

# Creating a `.gitignore` File

Create the file in the root of your repository.

```bash
touch .gitignore

```


------------------------------------------------------------------------

# 4. Stage the File

Add the file to the staging area

``` bash
git add example.txt
```

Or add all modified files:

``` bash
git add .
```


------------------------------------------------------------------------

# 5. Commit the Changes

Commit the staged files with a message.

``` bash
git commit -m "Added example.txt file"
```

A commit saves a snapshot of your changes in Git history. You need a 
commit message !

------------------------------------------------------------------------

# 6. Merge to your Branch

Push the changes to your branch

``` bash
git push origin feat/<feature name>
```

A push adds these changes to your branch in github

------------------------------------------------------------------------

# 7. Merge the Branch into Main

First switch to the main branch:

``` bash
git checkout main
```

Pull the latest changes:

``` bash
git pull origin main
```

Merge your branch:

``` bash
git merge feature-branch-name
```

------------------------------------------------------------------------

# 8. Push the Updated Main Branch

Upload the merged changes.

``` bash
git push origin main
```

------------------------------------------------------------------------

# Summary of Commands

``` bash
git clone <repo-url>
cd project-name
git checkout -b feature-branch-name
touch example.txt
git add .
git commit -m "Add new file"
git push origin feature-branch-name
git checkout main
git merge feature-branch-name
git push origin main
```

------------------------------------------------------------------------

# Optional Cleanup (Delete Branch)

After merging, you can delete the branch locally:

``` bash
git branch -d feature-branch-name
```

And remove it from the remote repository:

``` bash
git push origin --delete feature-branch-name
```

------------------------------------------------------------------------

# Git Workflow Overview

    Clone Repo
         ↓
    Create Branch
         ↓
    Make Changes
         ↓
    git add
         ↓
    git commit
         ↓
    git push
         ↓
    Merge Branch

------------------------------------------------------------------------

This is the standard Git workflow used by most development teams !!
