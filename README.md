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
