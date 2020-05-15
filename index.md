<div style="text-align: center;"><img 
src="https://raw.githubusercontent.com/MolSSI/molssi-branding-guidelines/master/logos/main_logo/molssi_main_logo.png" alt="MolSSI Logo" title="MolSSI 
Logo" height="100"/></div>

<div style="text-align: center;"><h1 style='margin: 0; padding: 0; border-bottom: none'>Git Cheat Sheet</h1></div>

## Git Configuration

| Command                                      | Description                                   |
| -------------------------------------------- | --------------------------------------------- |
| `git config --global user.name "Your Name"`  | Sets the author name for all future commits.  |
| `git config --global user.email "mole@cool"` | Sets the author email for all future commits. |
| `git config --global core.editor "nano"`     | Sets the default Git text editor to nano      |
| `git config --list`                          | Lists all current configuration settings.     |

## Essential Git

| Command                   | Description                                                  |
| ------------------------- | ------------------------------------------------------------ |
| `git init`                | Creates a new empty repository in the current folder.        |
| `git status`              | Summarizes the current state of the working tree and staging area. |
| `git log`                 | Shows all commits in reverse chronological order (most recent first). |
| `git add`                 | Stages one or more files.                                    |
| `git commit`              | Records changes in staging area in a new commit.             |
| `git commit -m "message"` | Shortcut to simultaneously commit and specify the commit message. |
| `git diff`                | Shows differences in files between working tree and HEAD.    |
| `git diff --cached`       | Shows differences in files  between staging area and HEAD.   |
| `git diff COMMIT_ID`      | Show differences in files between HEAD and a specific commit. |
| `git checkout COMMIT_ID`  | Temporarily reverts the repository to the state of a specific commit. |
| `git checkout master`     | Restores working tree when in DETACHED HEAD state.           |

## Git Branches

| Command                  | Description                                                  |
| ------------------------ | ------------------------------------------------------------ |
| `git branch`             | Lists existing branches.                                     |
| `git branch BRANCH`      | Creates a new branch BRANCH from the current HEAD.           |
| `git checkout BRANCH`    | Switches to the specified branch.                            |
| `git checkout -b BRANCH` | Creates a new branch and switches to it from the current HEAD. |
| `git merge BRANCH`       | Merges commits of BRANCH onto the history of the current branch. |
| `git branch -D BRANCH`   | Deletes branch BRANCH and its associated history.            |

## GitHub

| Command                   | Description                                                  |
| ------------------------- | ------------------------------------------------------------ |
| `git clone URL DIR`       | Clones (downloads) a repository from URL into a new directory DIR. |
| `git remote -v`           | Lists all remote repositories associated with the current repository. |
| `git remote add NAME URL` | Adds a remote repository NAME pointing to URL.               |
| `git remote rm NAME`      | Removes NAME from the list of tracked repositories.          |
| `git push NAME BRANCH`    | Copies commits of the current branch onto branch BRANCH of NAME. |
| `git pull NAME BRANCH`    | Merges commits of branch BRANCH of NAME onto the current branch. |

## Advanced Git

| Command                 | Description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| `git checkout -- FILE`  | Discards changes to a specific file in the working tree.     |
| `git reset HEAD FILE`   | Unstages a specific file (opposite of git add) but retains changes. |
| `git reset HEAD`        | Unstages all currently staged files.                         |
| `git reset --hard HEAD` | Erases **all** changes, reverting the repository to the state of HEAD. |

## Glossary

| Term         | Description                                                  |
| ------------ | ------------------------------------------------------------ |
| branch       | A self-contained collection of commits that represent a line of development. |
| commit       | A single point in the Git repository history.                |
| HEAD         | The commit at the tip of a branch or the most recent version of the repository. |
| remote       | A repository hosted elsewhere, often on the cloud.           |
| repository   | The collection of all files, changes (commits), and branches. |
| staging area | All the files and changes added to the staging area but not yet committed. |
| working tree | All files and changes not yet added to the staging area.     |
