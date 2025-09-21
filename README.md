<div align="center">
        <img height="80" src="https://cdn.simpleicons.org/git?viewbox=auto" alt="git"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
        <img height="80" src="https://cdn.simpleicons.org/github/white?viewbox=auto" alt="github"/>
</div>

<h1 align="center">Git & GitHub Tutorial 🚀</h1>

<div align="center">
        <a href="https://github.com/ChaitanyaShah26/git-github-tutorial">
          <img src="https://img.shields.io/github/stars/ChaitanyaShah26/git-github-tutorial?style=for-the-badge&logo=github&color=gold" alt="GitHub Stars" />
        </a>
        <a href="https://github.com/ChaitanyaShah26/git-github-tutorial">
          <img src="https://img.shields.io/github/forks/ChaitanyaShah26/git-github-tutorial?style=for-the-badge&logo=github&color=blue" alt="GitHub Forks" />
        </a>
        <a href="https://github.com/ChaitanyaShah26/git-github-tutorial/blob/main/LICENSE">
          <img src="https://img.shields.io/badge/license-MIT-darkgrey.svg?style=for-the-badge" alt="License" />
        </a>
</div>
<br>
<p align="center">
  Welcome to the ultimate guide to mastering Git and GitHub! 👋 This repository is designed to be a beginners guide to learn and get a handy reference for <b>Git</b> & <b>GitHub</b>.
</p>

## 🛠️ Getting Started: Setup

Before you can use Git, you need to set it up on your computer.

### 1. Create a GitHub Account 🌐
*   Go to [github.com](https://github.com) and sign up for a free account.

### 2. Install Git on Your Machine 💻
*   **Windows:** Download and install [Git for Windows](https://git-scm.com/download/win).
*   **Mac:** Open your terminal and run `git --version`. If you don't have it, it will prompt you to install Xcode Command Line Tools.
*   **Linux:** Open your terminal and use your distribution's package manager, e.g., `sudo apt-get install git`.

### 3. Configure Git ⚙️
After installing Git, introduce yourself! This information will be attached to every commit you make.
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```


## 🌟 Learn by Doing!
The best way to learn is by getting hands-on with the concept. In the steps below, you will practice the complete, basic workflow of contributing to an open-source project on GitHub.

**What you'll be doing:** You'll create your own copy of this project, download it to your computer, make a small change, and then propose that your change be added to the main project.

> [!NOTE]
> Don't worry if you don't understand what `forking`, `cloning` or `pull requests` mean yet. Just follow the steps, and you'll understand it all by the end of this tutorial!

**Get Started by following these steps:**
1.  **Star this repository:** Click the 'Star' button on the top right. ⭐
2.  **Fork this repository:** Click the 'Fork' button. This creates your own copy of this project. 🍴
3.  **Clone your fork:** On your forked repository's page, click the green "Code" button and copy the URL. Then, run this command in your terminal:
    ```bash
    git clone [the-url-you-copied]
    ```
4.  **Make a contribution:** Navigate into the new folder (`cd YOUR-REPONAME`) and add your name to the `CONTRIBUTING.md` file using a text editor.
5.  **Commit and Push your change:** Save the file, and then run these commands in your terminal:
    ```bash
    git add CONTRIBUTING.md
    git commit -m "Add [Your Name] to contributors"
    git push origin main
    ```
6.  **Open a Pull Request:** Go back to your forked repository on GitHub. You should see a yellow banner that says "This branch is 1 commit ahead of the original repository." Click the "Contribute" button, then "Open pull request." Follow the steps to submit your change.

Congratulations! You've just completed the core workflow of a GitHub contributor. 🎉



## 🧠 Core Git Concepts

### 1. What is Git & GitHub? 🤔
*   **Git** is a **distributed version control system**. Think of it as a program on your computer that takes "snapshots" (called commits) of your code. It allows you to track changes, go back to previous versions, and work on different features in parallel.
*   **GitHub** is a **cloud-based platform** that hosts your Git repositories. It adds a powerful web interface and tools for collaboration, like pull requests and issues, on top of Git.

> [!IMPORTANT]
> Run all the commands on your `cmd` or `git bash`

### 2. Repositories (Repos) 📂
A repository is a folder for your project that contains all its files and the entire history of changes.

> **🚀 Try it yourself!** Create a new project on your local machine.
> ```bash
> mkdir my-first-repo
> cd my-first-repo
> git init
> ```
> The `git init` command creates a hidden `.git` subfolder, which turns the directory into a Git repository.

### 3. The Commit Cycle: Add & Commit 🔄
A **commit** is a snapshot of your changes. It's a saved state of your code. This is a two-step process:
1.  **Staging (`git add`):** Choosing which changes you want to include in the next snapshot.
2.  **Committing (`git commit`):** Taking the snapshot with a descriptive message.

> **🚀 Try it yourself!** Let's make your first local commit.
> ```bash
> # In your 'my-first-repo' directory
> echo "Hello, Git!" > greeting.txt
> git status  # See that greeting.txt is "untracked"
> git add greeting.txt
> git status  # Now see it's "staged for commit"
> git commit -m "Add greeting file"
> git log     # See your commit history!
> ```

### 4. Branches in Git 🌳
A **branch** is an independent line of development. You create branches to work on new features or bug fixes without disturbing the main codebase (often the `main` branch).

> **🚀 Try it yourself!** Create a branch to test a new idea.
> ```bash
> # Create a new branch and switch to it
> git checkout -b new-idea
>
> # Make a change on this new branch
> echo "This is a new idea." >> greeting.txt
>
> # Commit the change on the 'new-idea' branch
> git add greeting.txt
> git commit -m "Experiment with a new idea"
>
> # Switch back to your main branch
> git checkout main
>
> # Notice that greeting.txt no longer contains "This is a new idea."
> cat greeting.txt
> ```

### 5. Merging ✅
**Merging** (`git merge`) combines the changes from one branch into another. This is how you integrate a new feature into your main codebase after you're done working on it.

> **🚀 Try it yourself!** Merge the `new-idea` branch you created.
> ```bash
> # Make sure you are on the main branch
> git checkout main
>
> # Merge the changes from 'new-idea' into 'main'
> git merge new-idea
>
> # Check the file - the changes are now here!
> cat greeting.txt
> ```

### 6. Merge Conflicts 🤯
This happens when Git can't automatically merge two branches, usually because they have conflicting changes on the *same line* of a file. You have to manually edit the file to resolve the conflict before the merge can be completed.

### 7. Stashing 🗄️
`git stash` temporarily shelves changes you've made so you can switch branches to work on something else without committing incomplete work.

> **🚀 Try it yourself!**
> ```bash
> # On your main branch, make an edit but don't commit
> echo "An unfinished thought..." >> thoughts.txt
> git status # Shows an uncommitted change
>
> # Stash the change to work on something else
> git stash
> git status # Your working directory is now clean!
>
> # Bring your changes back
> git stash pop
> git status # Your change is back
> ```

### 8. Issues 🎟️
**GitHub Issues** are a built-in bug and task tracker for your repository. They're perfect for keeping track of ideas, bugs, and tasks. You can create them on the "Issues" tab on your GitHub repository page.
