# 🐙 **Git & GitHub Command Cheat Sheet**

Master Git and GitHub with this comprehensive cheat sheet. From basics to advanced tricks, this guide has everything you need to manage and collaborate on code like a pro! 🚀  

---

## 🌟 **Getting Started with Git**

### 1. **Check Git Status**  
   ```bash
   git status
   ```
   *🛑 View modified, untracked, or staged files in your working directory.*

### 2. **Initialize a Git Repository**  
   ```bash
   git init
   ```
   *📂 Turn a project directory into a Git-tracked repository.*

### 3. **Clone a GitHub Repository**  
   ```bash
   git clone <repository_url>
   ```
   *📥 Copy a remote repository to your local machine.*

---

## 📤 **Making Changes Locally**

### 4. **Add Files to Staging Area**  
   ```bash
   git add <file_name>  # Add a specific file
   git add .            # Add everything
   ```
   *📂 Prepare changes for commit.*

### 5. **Commit Changes**  
   ```bash
   git commit -m "Your message"
   ```
   *💾 Save staged changes with a descriptive message.*

### 6. **Unstage Files**  
   ```bash
   git reset <file_name>
   ```
   *🚧 Remove files from staging without discarding changes.*

---

## 🌳 **Branching & Merging**

### 7. **Create and Switch to a Branch**  
   ```bash
   git checkout -b <branch_name>
   ```
   *🌿 Create and move to a new branch in one step.*

### 8. **Merge a Branch**  
   ```bash
   git merge <branch_name>
   ```
   *🔀 Combine changes from another branch into your current branch.*

### 9. **Delete a Branch**  
   ```bash
   git branch -d <branch_name>
   ```
   *🗑️ Remove a branch you no longer need.*

---

## 🌐 **Syncing with GitHub**

### 10. **Push Changes**  
   ```bash
   git push origin <branch_name>
   ```
   *🌐 Upload your local branch to the remote repository.*

### 11. **Pull Updates**  
   ```bash
   git pull origin <branch_name>
   ```
   *📥 Fetch and merge changes from the remote branch.*

---

## 🔧 **Advanced Git Commands**

### 12. **Rebase a Branch**  
   ```bash
   git rebase <branch_name>
   ```
   *🪄 Move your branch to start from the latest changes in another branch.*

   **Example Workflow:**  
   1. Switch to the feature branch: `git checkout feature-branch`  
   2. Rebase onto main: `git rebase main`

   *✨ This creates a cleaner commit history by replaying your commits on top of the target branch.*

---

### 13. **Squash Commits**  
   ```bash
   git rebase -i HEAD~<number_of_commits>
   ```
   *📦 Combine multiple commits into one to simplify history.*

   **Example Workflow:**  
   1. Use `git rebase -i HEAD~3` to squash the last 3 commits.  
   2. Mark commits as `squash` or `s` in the interactive editor.  
   3. Save and exit to merge the commits.

---

### 14. **Cherry-Pick a Commit**  
   ```bash
   git cherry-pick <commit_hash>
   ```
   *🍒 Apply a specific commit from one branch to another.*  

   **Example Workflow:**  
   1. Find the commit hash using `git log`.  
   2. Apply it to your branch: `git cherry-pick abc1234`.

---

### 15. **Stash Changes Temporarily**  
   ```bash
   git stash
   ```
   *🧳 Save your changes for later without committing.*

   **Retrieve Stashed Changes:**  
   ```bash
   git stash pop
   ```
   *🪄 Apply and remove the latest stash.*

---

### 16. **Amend the Last Commit**  
   ```bash
   git commit --amend -m "Updated commit message"
   ```
   *✏️ Edit the last commit message or add files you forgot to include.*

---

## 🔍 **Tracking and Troubleshooting**

### 17. **View Commit History**  
   ```bash
   git log
   git log --oneline
   ```
   *📜 View detailed or one-line commit history.*

### 18. **Check File Changes**  
   ```bash
   git diff <file_name>
   ```
   *🔍 Compare changes in a specific file.*

### 19. **Find the Commit That Introduced a Bug**  
   ```bash
   git bisect start
   git bisect bad
   git bisect good <commit_hash>
   ```
   *🐞 Automates binary search to pinpoint the bad commit.*

---

## ⚙️ **Customizing Git**

### 20. **Set Global User Info**  
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   ```
   *📇 Identify yourself for all repositories.*

### 21. **Alias Common Commands**  
   ```bash
   git config --global alias.co checkout
   git config --global alias.br branch
   git config --global alias.st status
   ```
   *⚡ Create shortcuts for frequent commands.*

---

## 🎉 **Bonus Tips**

- **Clean Up Old Branches Locally and Remotely**  
   ```bash
   git branch -d <branch_name>      # Delete local branch
   git push origin --delete <branch_name>  # Delete remote branch
   ```

- **Force Pull (Override Local Changes)**  
   ```bash
   git fetch origin
   git reset --hard origin/<branch_name>
   ```
   *⚠️ Warning: This overwrites your local changes.*

- **Track a Remote Branch Locally**  
   ```bash
   git checkout --track origin/<branch_name>
   ```
   *👣 Follows a remote branch for easy pulls and pushes.*

---

## 🚀 **Mastering Git Workflow**

1. Create a branch for new features:  
   ```bash
   git checkout -b feature/new-feature
   ```

2. Commit your work:  
   ```bash
   git add .
   git commit -m "Add new feature"
   ```

3. Push to GitHub:  
   ```bash
   git push origin feature/new-feature
   ```

4. Open a pull request on GitHub to merge into `main` or `develop`.

---

## ✨ **That's a Wrap!**

You’re now equipped with beginner and advanced Git skills. Start applying them to your projects, squash your bugs, and keep your commit history neat and clean. 🐙✨  

Got feedback or more advanced topics you'd like to cover? Let me know! 😊  

--- 