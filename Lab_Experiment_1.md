# DevOps Lab – Experiment 1

## Title

Introduction to Version Control, Git, GitHub, and Pushing a Project Using VS Code

## Aim

To understand the concept of Version Control Systems, learn the differences between Git and GitHub, and push a local project to GitHub using Visual Studio Code.

---

# 1. What is Version Control?

A **Version Control System (VCS)** is a software tool that records changes made to files over time. It enables developers to track modifications, restore previous versions, collaborate with multiple team members, and manage different versions of a project efficiently.

### Features

* Tracks file changes over time
* Maintains project history
* Restores previous versions
* Supports collaboration among developers
* Manages multiple development branches

### Advantages

* Prevents data loss
* Makes teamwork easier
* Simplifies debugging
* Maintains complete project history

---

# 2. How Git is Responsible for Version Control

Git is a **Distributed Version Control System (DVCS)** that manages source code by storing snapshots of the project after every commit.

### Working of Git

1. A repository is created using:

   ```bash
   git init
   ```

2. Files are modified in the working directory.

3. Changes are added to the staging area:

   ```bash
   git add .
   ```

4. Changes are permanently saved as a commit:

   ```bash
   git commit -m "Initial Commit"
   ```

5. Git stores every commit with a unique hash, creating a complete history of the project.

### Git Workflow

```
Working Directory
        │
        ▼
Staging Area
        │
        ▼
Commit History
        │
        ▼
Git Repository
```


---

# 3. Difference Between Git and GitHub

| Git                                          | GitHub                                                               |
| -------------------------------------------- | -------------------------------------------------------------------- |
| Git is a Distributed Version Control System. | GitHub is a cloud-based hosting platform for Git repositories.       |
| Used to track source code changes.           | Used to store and share Git repositories online.                     |
| Works offline.                               | Primarily requires an internet connection.                           |
| Installed on the local machine.              | Accessed through a web browser or desktop applications.              |
| Manages commits, branches, and merges.       | Provides Pull Requests, Issues, Actions, and collaboration features. |
| Developed by Linus Torvalds in 2005.         | Acquired by Microsoft in 2018.                                       |

---

# 4. Steps to Push a Project to GitHub Using VS Code

### Step 1: Open the project in Visual Studio Code

Open the project folder using **File → Open Folder**.

### Step 2: Open the Integrated Terminal

```
Terminal → New Terminal
```

### Step 3: Initialize Git

```bash
git init
```

### Step 4: Check Repository Status

```bash
git status
```

### Step 5: Add Files

```bash
git add .
```

### Step 6: Commit the Changes

```bash
git commit -m "Initial Commit"
```

### Step 7: Create a Repository on GitHub

Create a new repository from your GitHub account.

### Step 8: Connect Local Repository with GitHub

```bash
git remote add origin https://github.com/username/repository-name.git
```

### Step 9: Rename the Branch

```bash
git branch -M main
```

### Step 10: Push the Project

```bash
git push -u origin main
```

### Verify

Refresh the GitHub repository page to confirm that all project files have been uploaded successfully.

---

# Flowchart

```
                    START
                       │
                       ▼
          Create/Open Project Folder
                       │
                       ▼
                git init
      (Initialize Git Repository)
                       │
                       ▼
            Create / Modify Files
                       │
                       ▼
                 git status
      (Check Repository Status)
                       │
                       ▼
                 git add .
      (Stage Files for Commit)
                       │
                       ▼
      git commit -m "Commit Message"
      (Save Snapshot in Git History)
                       │
                       ▼
      Create Repository on GitHub
                       │
                       ▼
       git remote add origin <repo-url>
                       │
                       ▼
            git branch -M main
                       │
                       ▼
       git push -u origin main
                       │
                       ▼
      Project Successfully Uploaded
             to GitHub Repository
                       │
                       ▼
                      END

```

---

# Result

Successfully studied the concepts of Version Control, Git, and GitHub, understood the differences between Git and GitHub, and successfully pushed a local project to GitHub using Visual Studio Code.

---

# Conclusion

Git is a distributed version control system that helps developers track changes, manage versions, and collaborate efficiently. GitHub is a cloud-based platform that hosts Git repositories and provides collaboration features. Using Visual Studio Code along with Git simplifies source code management and enables seamless project synchronization with GitHub.
