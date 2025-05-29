# Table of Contents
### Prerequisites
### Creating a Repository 
### Adding Notes to the Repository
### Committing Changes with Clear Messages
### Creating and Switching Branches
### Resolving Merge Conflicts
### Cloning a Repository
### Forking a Repository

### Prerequisites
- A GitHub account.
- Git installed on your local machine Download Git.
- Basic knowledge of the command line (Terminal for macOS/Linux, Command Prompt/PowerShell for Windows/Gitbash).

### Creating a Repository
- Log in to GitHub: Go to GitHub and sign in.
- Create a New Repository
- Click the + icon in the top-right corner and select New repository.
- Enter a repository name (e.g., my-repo).
- Choose Public or Private visibility.
- Optionally, add a description and initialize with a README.
- Click Create repository.
### Local Setup:
- Clone the repository to your local machine (see Cloning a Repository)
- Alternatively, create a local folder and initialize Git:
``` bash 
mkdir my-repo
cd my-repo
git init
git remote add origin https://github.com/your-username/my-repo.git
```
### Adding Notes to the Repository
- Create a file (e.g., notes.txt) in your repository folder
``` bash 
touch notes.txt
```
- Add content to notes.txt using a text editor or command line
``` bash
echo "My project notes" > notes.txt ```
- Stage the file for commit
``` bash 
git add notes.txt
```
### Committing Changes with Clear Messages
- Commit changes with a descriptive message
``` bash 
git commit -m "Add initial notes to notes.txt"
```
- Push changes to GitHub
``` bash
git push -u  origin new-branch
```
### Creating and Switching Branches
- Create a New Branch
``` bash 
git branch feature-b
```
- Or create and switch to the branch in one command
```
bash 
git checkout -b feature-b
```
## Switch Between Branches
- Switch to the main branch
``` bash
git checkout new-branch
```
## Switch to feature-b
``` bash
git checkout feature-b
```
## switch to previous branch
``` bash 
git checkout -
```
### Make changes in feature-branch, commit, and push
```
bash
echo "Feature notes" >> notes.txt
git add notes.txt
git commit -m "Add feature notes in feature-branch"
git push -u origin feature-b
```
## Resolving Merge Conflicts
- Create a Conflict
``` bash
git checkout main
echo "Main branch changes" >> notes.txt
git add notes.txt
git commit -m "Update notes in main"
git push origin main
```
## Switch to feature-branch and edit the same line in notes.txt
``` bash 
git checkout feature-branch
echo "Feature branch changes" >> notes.txt
git add notes.txt
git commit -m "Update notes in feature-branch"
git push origin feature-branch




