## 🖥️ CMD (Command Prompt) Commands

| Command | Description | Example |
|----------|--------------|----------|
| `dir` | Lists files and directories. | `dir` |
| `cd` | Changes directory. | `cd project` / `cd ..` |
| `mkdir` | Creates a directory. | `mkdir new_folder` |
| `rmdir` | Deletes an empty directory. | `rmdir old_folder` |
| `del` | Deletes a file. ⚠️ | `del file.txt` |
| `copy` | Copies files. | `copy file.txt D:\backup` |
| `move` | Moves or renames files. | `move file.txt new_folder\` |
| `cls` | Clears the screen. | `cls` |
| `exit` | Exits CMD. | `exit` |
| `type` | Displays file content. | `type README.md` |

---

## 🧰 Git Commands (Version Control)

### 🔧 Configuration

| Command | Description | Example |
|----------|--------------|----------|
| `git config --global user.name` | Sets username. | `git config --global user.name "Josep"` |
| `git config --global user.email` | Sets email. | `git config --global user.email "you@example.com"` |
| `git config --list` | Shows configuration. | `git config --list` |

---

### 🏁 Repository Setup

| Command | Description | Example |
|----------|--------------|----------|
| `git init` | Initializes a new repository. | `git init` |
| `git clone` | Clones an existing repo. | `git clone https://github.com/user/repo.git` |

---

### 💾 Change Management

| Command | Description | Example |
|----------|--------------|----------|
| `git status` | Shows repo status. | `git status` |
| `git add` | Adds files to staging area. | `git add file.py` / `git add .` |
| `git commit -m` | Saves changes with message. | `git commit -m "Added feature"` |
| `git log` | Shows commit history. | `git log` |
| `git diff` | Shows file differences. | `git diff` |
| `git restore` | Restores modified files. | `git restore file.py` |

---

### 🌿 Branch Management

| Command | Description | Example |
|----------|--------------|----------|
| `git branch` | Lists branches. | `git branch` |
| `git branch feature` | Creates new branch. | `git branch feature-login` |
| `git switch feature` | Switches branch. | `git switch main` |
| `git merge feature` | Merges branch into current. | `git merge feature-login` |
| `git branch -d feature` | Deletes branch. | `git branch -d feature-login` |

---

### 🔄 Remote Repositories

| Command | Description | Example |
|----------|--------------|----------|
| `git remote -v` | Shows remote repos. | `git remote -v` |
| `git push` | Pushes commits to remote. | `git push origin main` |
| `git pull` | Pulls and merges changes. | `git pull origin main` |
| `git fetch` | Fetches changes without merging. | `git fetch origin` |

---

### 🧹 Other Useful Commands

| Command | Description | Example |
|----------|--------------|----------|
| `git stash` | Temporarily saves changes. | `git stash` |
| `git stash pop` | Restores stashed changes. | `git stash pop` |
| `git revert <commit>` | Reverts a commit. | `git revert 3a5b6c7` |
| `git reset --hard <commit>` | Resets to previous state ⚠️ | `git reset --hard HEAD~1` |
| `git tag` | Lists or creates tags. | `git tag v1.0` |

---

👨‍💻 **Author:** Josep  
📚 **Purpose:** A personal knowledge base and reference for Python developers.
