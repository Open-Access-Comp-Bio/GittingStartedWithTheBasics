# Gitting Started With The Basics
Hey there!
Git is an incredible tool that can feel very intimidating for someone new. This guide will give you the foundamental basics: Set up, create a repo, and make your first commit.

## Table of Contents
- [Setting up Git](#setting-up-git)
- [Create a Repository](#create-a-repository)
- [Staging and Committing](#stage-and-commit-changes)
- [Push to GitHub](#push-to-github)
- [Make Changes Later](#make-changes-later)
- [Pull Changes from GitHub](#pull-changes-from-github)


## Setting Up Git
Before you can start using Git, you need to set it up on your computer. Follow these steps:
1. **Install Git**: Download and install Git from [git-scm.com](https://git-scm.com/). Follow the installation instructions for your operating system.

2. **Verify Installation**: To ensure Git is installed correctly, run:
   ```bash
   git --version
   ```
   You should see the installed version of Git.

3. **Configure Git**: Open your terminal (Command Prompt, PowerShell, or Git Bash) and set your username and email address. These will be associated with your commits.
    ```bash
    git config --global user.name "githubusername"
    git config --global user.email "your@email.com"
    ```
## Create a Repository
You can create a new Git repository (repo) either locally on your computer or on Github.
### Via Git
```bash
mkdir my-repo-name
cd my-repo-name
git init
```
**Note**: When you run `git init`, it creates a hidden `.git` directory in your project folder. This directory contains all the necessary files and metadata for your Git repository. So don't forget to run this command!

### Via GitHub
The official Github documentation covers how to create a [repo online](https://docs.github.com/en/get-started/quickstart/create-a-repo).

## Stagging and Committing Changes
`Staging` and `committing` are going to be your two most used actions.
When you're `staging` your telling `Git` "I want the following files to be pushed to the repo". 

Let's now create a really simple `README.md`. 
You can either use your favorite text editor or run the following command in your terminal:

```bash
echo "Hello, World!" >> README.md
```

Now, let's stage the `README.md` file:

```bash
git add README.md
``` 
You can stage multiple files at once by using `git add .` to stage all changes in the current directory. **BE CAREFUL** with this command, as it will stage all changes, including **deletions, modifications, and any test outputs!**

