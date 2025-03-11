# Connecting Your Project to GitHub and Managing Updates

## 1. Install and Set Up Git
Check if Git is installed by running the following command in **VS Code's terminal** (`Ctrl + ~`):

```sh
git --version
```
If not installed, [download and install Git](https://git-scm.com/downloads).

Set up your Git user information:

```sh
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

---

## 2. Initialize Git in Your Project
Open your project folder in **VS Code**, then run:

```sh
git init
```

This initializes a Git repository in your project folder.

---

## 3. Create a GitHub Repository
1. Go to [GitHub](https://github.com/)
2. Click **New Repository**.
3. Enter a repository name.
4. **Do NOT check "Initialize with a README"** (since your project already exists locally).
5. Click **Create Repository**.
6. Copy the repository **HTTPS or SSH URL**.

---

## 4. Connect Your Local Project to GitHub
In VS Code’s terminal, run:

```sh
git remote add origin <your-repo-url>
```
Example:

```sh
git remote add origin https://github.com/your-username/your-repo.git
```

To verify the remote connection:

```sh
git remote -v
```

---

## 5. Add, Commit, and Push Your Code
### First Commit & Push
```sh
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```

---

## 6. Pull Latest Changes from GitHub
If you make changes on GitHub and want to update your local project:

```sh
git pull origin main
```

---

## 7. Workflow for Ongoing Updates
1. **Check the status of changed files**:
   
   ```sh
   git status
   ```

2. **Add changes to staging**:
   
   ```sh
   git add .
   ```

3. **Commit changes**:
   
   ```sh
   git commit -m "your commit message"
   ```

4. **Push to GitHub**:
   
   ```sh
   git push origin main
   ```

---

## 8. Pull Updates from GitHub Before Working
Before making new changes, always pull the latest version to avoid conflicts:

```sh
git pull origin main
```

---

## 9. Handling Merge Conflicts
If Git detects conflicts after pulling:

1. Open conflicting files in **VS Code**.
2. Choose between **"Accept Incoming Changes"**, **"Accept Current Changes"**, or manually edit.
3. Once resolved, **stage** the files and commit:

   ```sh
   git add .
   git commit -m "Resolved merge conflict"
   git push origin main
   ```

---

Now your project is connected to GitHub, and you can efficiently manage updates with **commit, push, and pull**! 🚀
