# 🐙 **Git & GitHub Command Cheat Sheet**

Git and GitHub are your trusty sidekicks in version control and collaboration. Below is an **enhanced guide** to mastering the most frequently used commands for all your development needs. Let’s commit to learning! 🚀  

---

## 🌟 **Getting Started with Git**

### 1. **Check Git Status**  
   ```bash
   git status
   ```
   *🛑 See what’s happening in your working directory: which files are modified, untracked, or ready to commit.*

### 2. **Initialize a Git Repository**  
   ```bash
   git init
   ```
   *📂 Converts a directory into a Git-tracked project.*  

### 3. **Clone a GitHub Repository**  
   ```bash
   git clone <repository_url>
   ```
   *📥 Copies a remote repository to your local machine.*  

---

## 📤 **Making Changes Locally**

### 4. **Add Changes to Staging Area**  
   ```bash
   git add <file_name>    # Add a specific file
   git add .              # Add everything
   ```
   *📂 Moves changes to the staging area, preparing them for commit.*

### 5. **Commit Changes**  
   ```bash
   git commit -m "Your descriptive message"
   ```
   *💾 Saves the changes to the repository with a message explaining why.*

### 6. **Undo Changes Before Committing**  
   ```bash
   git checkout -- <file_name>
   ```
   *🔄 Reverts changes in a file back to the last committed version.*

---

## 🌳 **Branching Made Easy**

### 7. **Create a New Branch**  
   ```bash
   git branch <branch_name>
   ```
   *🌱 Starts a new branch for experimenting with changes.*

### 8. **Switch to a Branch**  
   ```bash
   git checkout <branch_name>
   ```
   *🔄 Switches to another branch.*  

### 9. **Create & Switch to a New Branch (Shortcut)**  
   ```bash
   git checkout -b <branch_name>
   ```
   *⚡ Combines creating and switching into one command.*

### 10. **Delete a Branch**  
   ```bash
   git branch -d <branch_name>
   ```
   *🗑️ Deletes a branch that you no longer need.*

---

## 🌐 **Connecting to GitHub**

### 11. **Push Changes to GitHub**  
   ```bash
   git push origin <branch_name>
   ```
   *🌐 Uploads your local branch to the remote repository.*  

### 12. **Pull Updates from GitHub**  
   ```bash
   git pull origin <branch_name>
   ```
   *📥 Syncs your branch with the latest changes from the remote.*  

### 13. **Set Upstream for a Branch**  
   ```bash
   git push --set-upstream origin <branch_name>
   ```
   *🔗 Links your branch to the remote branch for future pushes.*

---

## 🤝 **Collaborating with Others**

### 14. **Fork a Repository**  
   *🔗 Creates your personal copy of someone else’s repository. Use the "Fork" button on GitHub.*

### 15. **Create a Pull Request**  
   *📬 Suggest changes to the original repository. Go to GitHub and click "New Pull Request."*

### 16. **Merge Branches Locally**  
   ```bash
   git merge <branch_name>
   ```
   *🔀 Combines changes from one branch into another (usually `main`).*

---

## 🧹 **Fixing Mistakes**

### 17. **Unstage a File**  
   ```bash
   git reset <file_name>
   ```
   *🚧 Removes a file from staging without modifying it.*  

### 18. **Undo the Last Commit**  
   ```bash
   git reset --soft HEAD~1  # Keep changes staged
   git reset --hard HEAD~1  # Discard changes entirely
   ```
   *⚠️ Use `--hard` with caution—it permanently deletes changes.*

### 19. **Remove Untracked Files**  
   ```bash
   git clean -f
   ```
   *🗑️ Deletes files that Git isn’t tracking.*

---

## 🔍 **Tracking History**

### 20. **View Commit History**  
   ```bash
   git log
   ```
   *📜 Shows all commits in your repository.*  

### 21. **View File Changes**  
   ```bash
   git diff <file_name>
   ```
   *🔍 Shows changes made to a specific file.*

### 22. **Compare Two Branches**  
   ```bash
   git diff <branch1>..<branch2>
   ```
   *📊 Highlights differences between two branches.*

---

## ⚙️ **Customizing Git**

### 23. **Set Your User Info Globally**  
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your_email@example.com"
   ```
   *📇 Identifies you in every repository.*

### 24. **Set a Default Editor**  
   ```bash
   git config --global core.editor "code --wait"  # Example: VS Code
   ```
   *📝 Specifies your preferred editor for commit messages.*

### 25. **Check Your Configurations**  
   ```bash
   git config --list
   ```
   *⚙️ Displays your current Git setup.*

---

## 🎉 **Level Up Your Workflow**

- **Alias Your Most-Used Commands:**  
   Add shortcuts to save typing time:  
   ```bash
   git config --global alias.co checkout
   git config --global alias.br branch
   git config --global alias.ci commit
   git config --global alias.st status
   ```
   *⚡ Example: `git co main` instead of `git checkout main`.*

- **Keep It Clean with Prune:**  
   ```bash
   git remote prune origin
   ```
   *🌐 Cleans up remote branches that no longer exist.*  

---

## ✨ **That’s It!**

This cheat sheet has everything you need to **push, pull, merge, and commit like a pro**. Save it, share it, and let GitHub be your collaborative superpower. 🐙✨  

Got suggestions? Let me know! 😊  

---