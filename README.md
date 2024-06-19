

# Junior Developer Git Interview Questions

## 1. What is Git and why is it used?
**Question:** Can you explain what Git is and why it is used in software development?

**Answer:** Git is a distributed version control system used to track changes in source code during software development. It allows multiple developers to work on a project simultaneously without overwriting each other's changes. Git enables branching, merging, and tracking of changes, which facilitates collaboration, version management, and ensures the integrity of the codebase.

## 2. How do you initialize a new Git repository?
**Question:** How do you create a new Git repository in an existing project directory?

**Answer:** To initialize a new Git repository in an existing project directory, navigate to the project directory in your terminal and run the command:
```sh
git init
```
This command creates a new subdirectory named `.git` that contains all the necessary files for the repository.

## 3. What is the difference between `git pull` and `git fetch`?
**Question:** Can you explain the difference between `git pull` and `git fetch`?

**Answer:** `git fetch` downloads updates from the remote repository to your local repository but does not automatically merge them into your working directory. It allows you to review the changes before integrating them. `git pull` is a combination of `git fetch` and `git merge`, meaning it fetches the changes and automatically merges them into your current branch.

## 4. How do you create a new branch and switch to it?
**Question:** What are the commands to create a new branch and switch to it?

**Answer:** To create a new branch, use:
```sh
git branch <branch-name>
```
To switch to the newly created branch, use:
```sh
git checkout <branch-name>
```
Alternatively, you can combine both actions into one command:
```sh
git checkout -b <branch-name>
```

## 5. How do you stage and commit changes?
**Question:** What commands do you use to stage changes and commit them?

**Answer:** To stage changes, use:
```sh
git add <file-name>
```
or to stage all changes:
```sh
git add .
```
To commit the staged changes, use:
```sh
git commit -m "commit message"
```
This stages the changes and records them in the repository with a descriptive message.

## 6. How do you revert a commit?
**Question:** What command do you use to revert a commit?

**Answer:** To revert a commit, use:
```sh
git revert <commit-hash>
```
This command creates a new commit that undoes the changes made by the specified commit. The `<commit-hash>` is the identifier of the commit you want to revert.

## 7. How can you view the history of commits in a repository?
**Question:** How do you view the commit history of a repository?

**Answer:** To view the commit history, use:
```sh
git log
```
This command shows the list of commits along with their hash, author, date, and commit message. For a more compact and visually appealing log, you can use:
```sh
git log --oneline --graph --decorate --all
