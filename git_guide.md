# Git Basics & Working on the **dirty** Branch

This guide shows how to use common Git commands, switch to the `platform-efs2-dirty-branch`, and understand pull requests.

---  

## 1 Check Your Current Branch  

```bash
git branch
```  

The branch with an asterisk (`*`) is the one you’re currently on.

---  

## 2️ Switch to the **dirty** Branch  

```bash
git switch platform-efs2-dirty-branch
```  

If the branch does not exist locally, create and switch to it:

```bash
git checkout -b platform-efs2-dirty-branch origin/platform-efs2-dirty-branch
```

---  

## 3️ Make Changes & Stage Files  

Edit your files as needed, then stage the changes:

```bash
git add <file‑path>          # stage a specific file
git add .                    # stage all modified files
```

---  

## 4️ Commit Your Changes  

```bash
git commit -m "Brief description of what you changed"
```  

*Use a clear, concise message so teammates understand the purpose of the commit.*

---  

## 5️ Push to the Remote Repository  

```bash
git push origin platform-efs2-dirty-branch
```  

Your commits are now on the remote `platform-efs2-dirty-branch`.

---  

## 6️ What Is a Pull Request (PR)?  

A **pull request** is a request to merge changes from one branch (e.g., `platform-efs2-dirty-branch`) into another branch (often `main` or `develop`).  

- **Creates a review workflow:** teammates can comment, approve, or request changes.  
- **Keeps history clean:** the merge is recorded as a single commit (or a series of commits) in the target branch.  
- **Does not affect other branches** until it is merged.

> **Important:** Do **not** click “Compare & pull request” if you only want to work on the dirty branch. Creating a PR will propose merging your changes into another branch, which may alter code you’re not ready to share.

---  

## 7️ Quick Reference Cheat Sheet  

| Action                     | Command(s)                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| View current branch        | `git branch`                                                                |
| Switch to existing branch  | `git switch platform-efs2-dirty-branch`                                     |
| Create & switch new branch | `git checkout -b platform-efs2-dirty-branch origin/platform-efs2-dirty-branch` |
| Stage changes              | `git add <file>` or `git add .`                                             |
| Commit                     | `git commit -m "Your message"`                                              |
| Push to remote             | `git push origin platform-efs2-dirty-branch`                                |
| Open a PR (GitHub UI)      | Click **Compare & pull request** → fill details → **Create pull request**   |

---  

## 8️ Example Workflow  

```bash
# 1. Verify where you are
git branch

# 2. Switch to the dirty branch
git switch platform-efs2-dirty-branch

# 3. Edit a file (e.g., src/login.js)
#    (use your editor of choice)

# 4. Stage the change
git add src/login.js

# 5. Commit with a helpful message
git commit -m "Fix login validation edge case"

# 6. Push to the remote dirty branch
git push origin platform-efs2-dirty-branch
```

Now the changes are safely on the `platform-efs2-dirty-branch`. When the team is ready, they can create a pull request to merge these updates into the main development line.

---  

*Dirty coding!*
