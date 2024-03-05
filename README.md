```sh
Just doing some funny stuff in this repo with the git commands for learning and prepare for exam ;)
```


## Git HIdden Folder
There is a hidden folder called `.git` which tells you that your project is a git repo.

if we want to create a git repo in a new project we created th efolder and initialize that repo using `git init`:
```

git init
```
# Cloning
We can clone three ways: HTTPS, SSH, Github CLI
Since we are using Github Codespace we'll a create temporary directory in our workspace
```sh
for exmp:
mkdir /github foundation exam course/new-project
cd github foundation exam course/new-project
touch Readme.md
code Readme.md (in vscode)
git status
git add Readme.md
# makes changes to readme.md
git commit -m "add readme file"
```

# HTTPS
```sh
- git clone https://github.com/aidinfk/github-foundation-exam-course.git
- cd github-foundation-exam-course
```

> You need to generate a Personal Access Token(PAT) => https://github.com/settings/tokens/new
- You will use the PAT as your password when you login
- Give it access to contents for commits

### SSH
```ssh
git clone git@github.com:aidinfk/Github-Examples.git
cd Github-Examples
```

# Commits
When we want to commit code we can write git commit which wil open up the commit edit message in the editor of choice.
```sh
git commit
```
Set the global editor:
```sh
git config --global core.editor emacs
```
Make a commit and commit message without opening an editor
```sh
git commit -m "add another exclamation"
```

# Branches

# Remotes

# Strashing

# Merging

# Add
When we want to stage changes that will be included in the commit, we use the . to add all possible files.

```
git add Readme.md
git add .
```

# Reset
Reset allows you to move staged changes to be unstaged.
This is useful when you want to revert all files not to be not commited!

```
git add .
git reset
```
> git reset will revert a git add .

# Status
Git status shows you what files will or will not be commited.

```
git status
```

# Gitconfig file
The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

Showing the contents of our .gitconfig file:
```
git config --list
```

When yopu first install Git on the machine you are supposed to set up your name and email:
```sh
git config --global user.name "Your Name"
git config --global user.email youremail@example.com
```
## Log
git log will show recent get commits to the git tree

## Push
when we want to push a repo to our remote origin
```
git push
```