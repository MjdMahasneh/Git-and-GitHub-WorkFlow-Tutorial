# Git and GitHub Workflow

To contribute to a repository where you have <span style="color: red;"> **Write Access**</span>, i.e., collaboration access, follow these steps:


## Setting Up and Making Changes

### Clone the Repository
First, clone the repository to your local machine if you haven't already:
```bash
git clone <repository-url>
```

Replace `<repository-url>` with the actual URL of your GitHub repository.



### Create a New Branch
Create a new branch to safely make your changes without affecting the main branch (you might need to `cd` into the repository directory first):
```bash
git checkout -b <new-branch-name>
```
Replace `<new-branch-name>` with a descriptive name for your branch.

### Make Changes
Edit, add, or delete files as needed in your project using your preferred code editor.

## Staging and Committing Changes

### Stage Changes
Add your changes to the staging area, preparing them for a commit:

```bash
git add .
```

Or stage files individually:
```bash
git add <file-path>
```

### Commit Changes
Commit your staged changes, which saves them in your local repository:

```bash
git commit -m "Descriptive message about the changes"
```

## Pushing Changes and Creating a Pull Request

### Push Changes
Upload your local branch and its commits to GitHub:
```bash
git push origin <new-branch-name>
```


### Create a Pull Request
- Go to your repository on GitHub.
- You'll see a prompt to create a pull request for the branch you just pushed. Click "Compare & pull request".
- Review the changes, add a description to your pull request, and then submit it.

## Reviewing and Merging the Pull Request

### Review and Discuss
Team members review the pull request, discuss any necessary changes, and approve the changes.

### Merge the Pull Request
- Once approved, merge the pull request into the main branch on GitHub.
- Click "Merge pull request" and then "Confirm merge".

## Syncing Local Repository

### Pull Changes to Local Main Branch
After merging, update your local main branch:

```bash
git checkout main
git pull origin main
```

This summary outlines a typical workflow for individual or team projects using Git and GitHub, covering everything from initial setup to syncing your local environment after changes have been integrated.


---


# Git and GitHub Workflow for Forked Repositories

To contribute to a repository where you have <span style="color: red;"> **no Write Access**</span>, e.g., public contributor, follow these steps:

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
