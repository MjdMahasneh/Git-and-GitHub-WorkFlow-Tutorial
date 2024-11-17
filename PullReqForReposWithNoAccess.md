# Git and GitHub Workflow for Forked Repositories

To contribute to a repository where **you don't have write access**, follow these steps:

- #### Fork the Repository

Go to the GitHub page of the repository you want to contribute to.
Click the "Fork" button (top-right corner). This creates your copy of the repository.


- #### Clone Your Fork

Clone your forked repository to your local machine:
```bash
git clone <your-forked-repo-url>
```
Replace <your-forked-repo-url> with the URL of your fork.


- #### Create a New Branch

Navigate into the cloned repository folder:
```bash
cd <repository-folder>
```

Create a new branch for your changes:

```bash
git checkout -b <new-branch-name>
```

- #### Make and Commit Changes

Make your changes using a text editor or IDE.


- #### Stage your changes:
```bash
git add .
```

- #### Commit the changes with a message:

```bash
git commit -m "Descriptive message about the changes"
```

- #### Push Changes to Your Fork

Push your branch to your forked repository:
```bash
git push origin <new-branch-name>
```

- #### Create a Pull Request

Go to the original repository on GitHub.
Click "Pull Requests", then "New Pull Request".
Select your fork and branch as the source, and the original repository's branch (usually main) as the target.
Add a description and submit the pull request.

- ## Optional: Stay Updated

If the original repository changes while you work:

- #### Set the original repo as an upstream remote:

```bash
git remote add upstream <original-repo-url>
```

- #### Fetch and merge updates:

```bash
git fetch upstream
git merge upstream/main
```



- #### Push the updates to your fork:

```bash
git push origin main
```

This process ensures your contribution is clean and ready for review!