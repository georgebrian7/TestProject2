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
git branch to-the-exiles
```
- Or create and switch to the branch in one command
```
bash 
git checkout -b to-the -exiles
```
## Switch Between Branches
- Switch to the main branch
``` bash
git checkout new-branch
```
## Switch to to-the-exiles
``` bash
git checkout 
```
## switch to previous branch
``` bash 
git checkout -
```
### Make changes in to-the-exiles, commit, and push
```
bash
echo "Feature notes" >> notes.txt
git add notes.txt
git commit -m "Add feature notes in to-the-exiles"
git push -u origin to-the-exiles
```
## Resolving Merge Conflicts
- Create a Conflict
- In new-branch, edit notes.txt
``` bash
git checkout new-branch
echo "Main branch changes" >> notes.txt
git add notes.txt
git commit -m "Update notes in new-branch"
git push  -u origin to-the-exiles
```
## Switch to to-the-exiles and edit the same line in notes.txt
``` bash 
git checkout feature-branch
echo "to-the-exiles changes" >> notes.txt
git add notes.txt
git commit -m "Update notes in to-the-exiles"
git push -u origin to-the-exiles 
```
## Merge with Conflict
- Switch to new-branch and attempt to merge to-the-exiles:
``` bash
git checkout new-branch
git merge to-the-exiles
```
- Git will indicate a conflict in notes.txt.
- Resolve the Conflict
- Open notes.txt in a text editor. You'll see conflict markers: ``` <<<<<<< HEAD new-branch changes, to-the-exiles changes,to-the-exiles ```
- Edit the file to keep desired changes (e.g., combine both)
- Stage and commit the resolved file
``` bash 
git add notes.txt
git commit -m "Resolve merge conflict in notes.txt"
git push -u origin new-branch
```
- Delete the Feature Branch (optional)
``` bash 
git branch -d to-the-exiles
git push origin --delete to-the-exiles
```
## Cloning a Repository
- Copy the repository URL from GitHub (e.g., https://github.com/rahim8050/TestProject).
## Clone the repository to your local machine
-create a folder on where you want to clone the repository
- open the folder with gitbash
## run the following command
``` bash
 git clone https://github.com/rahim8050/TestProject
```
- Navigate to the cloned folder
 ``` bash 
 cd TestProject
 ```
 ## Forking a Repository
 - Go to the repository you want to fork on GitHub (e.g., https://github.com/rahim8050/TestProject ).










