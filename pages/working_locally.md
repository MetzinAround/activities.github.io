---
layout: default
title: Working Locally With GitHub
nav_order: 5
permalink: /local/
---

# 🖥️ WORKING LOCALLY WITH GITHUB

Learning to work on GitHub from your own computer is one of the most important skills you can build as a developer (or really, anyone who uses GitHub regularly!). This lesson will walk you through installing the tools you need, connecting them to your GitHub account, and running through the core local workflow: creating repos, making branches, committing changes, and pushing it all up to GitHub. You'll finish by cloning the repo you made in the [Profile README activity](/profile-readme/)!

---

## Prerequisites

Before starting this lesson, you should:

- Have **completed (or be familiar with) the Profile README activity** — you'll be cloning that repo at the end of this lesson! If you haven't done it yet, [complete it here](/profile-readme/).
- Be comfortable navigating your computer's file system (opening folders, knowing where your Desktop or Documents folder is).
- Have basic familiarity with what a repository is on GitHub.com.

---

## What You'll Learn

By the end of this lesson you will be able to:

- Install and configure **Git**, **GitHub Desktop**, and **VS Code**
- Connect (authenticate) GitHub Desktop to your GitHub account
- Create a new repository **locally** and push it to GitHub
- Create and switch between **branches** locally
- **Clone** an existing GitHub repository to your computer

---

## Part 1: Installing Your Tools

You'll be installing three tools:

| Tool | What it does |
|------|-------------|
| **VS Code** | A free code editor where you'll make changes to your files |
| **Git** | The underlying version control software everything else relies on |
| **GitHub Desktop** | A visual app that makes using Git with GitHub much easier |

You can skip any of these if you know you already have it installed. 

---

### 🔧 Step 1: Install VS Code

VS Code (Visual Studio Code) is a free text editor made by Microsoft. You'll use it to edit files on your computer.

1. Go to [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Click the large **Download** button. The site auto-detects your operating system.
3. Open the downloaded file and follow the installation steps. Default options are fine for everyone.
4. Once installed, open VS Code to make sure it launches correctly. You should see a welcome screen.

> 💡 **Optional — Sign into GitHub in VS Code:** If you later want to use VS Code's built-in GitHub features (like Copilot or the GitHub Pull Requests extension), you can sign in by clicking the **Accounts** icon in the bottom-left corner of VS Code. This isn't needed for this lesson — GitHub Desktop handles all your GitHub authentication here.

---

### 🔧 Step 2: Install Git

Git is the engine under the hood. Even though you'll mostly use GitHub Desktop, Git must be installed for everything to work.

**📌 Windows**

1. Go to [https://git-scm.com/download/win](https://git-scm.com/download/win) and click **"Click here to download"** to get the latest 64-bit version. (If you're unsure which to pick, 64-bit is correct for most modern Windows computers.)

2. Once downloaded, open the file (it will look something like `Git-2.x.x-64-bit.exe`). If Windows asks *"Do you want to allow this app to make changes?"*, click **Yes**.

3. The installer has several screens — here's what to do:
   - **License & Install Location:** Click **Next** to accept the defaults.
   - **Choosing the default editor:** Git will suggest *Vim* as the default editor — this is not beginner-friendly. We recommend changing this to **VSCode** (or another editor you're comfortable with) using the dropdown, then click **Next**.
   - **All remaining screens:** Leave everything else on the default settings and keep clicking **Next**, then click **Install**.

4. Click **Finish** when the installation completes.

**To verify Git installed correctly:**

1. Open a Command Prompt window: press the **Windows key**, type `cmd`, and press **Enter**.

2. Type the following and press **Enter**:
   ```
   git --version
   ```

3. You should see something like `git version 2.x.x`. If you do — Git is installed! ✅

> 💡 Git also installs **Git Bash**, a terminal app you can use instead of Command Prompt. You'll find it by searching "Git Bash" in the Start menu.

---
**📌 Mac**

1. Open the **Terminal** app (press `Command + Space`, type `Terminal`, and press `Enter`).

2. Check if Git is already installed by typing the following and pressing `Enter`:
   ```
   git --version
   ```
   - If you see a version number (e.g., `git version 2.39.0`) — you're all set! ✅
   - If Git is not installed, macOS will automatically pop up a prompt to install the **Xcode Command Line Tools** — click **Install** and follow the prompts. Git will be installed as part of this.

3. If the automatic prompt doesn't appear, install Git using one of these options:

   **Option A — Homebrew (recommended):**
   Homebrew is a free package manager for Mac. It makes downloading and installing developer tools and other packages easier to use. It's up to you whether you install Homebrew or not. To install, paste the following into Terminal and press `Enter`:
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
   Once Homebrew is installed, type the following into Terminal and press `Enter`:
   ```
   brew install git
   ```

   **Option B — Binary Installer:**
   Go to [https://git-scm.com/download/mac](https://git-scm.com/download/mac), click the download link under **Binary installer**, open the `.pkg` file that downloads, and follow the installation steps.

4. Once finished, run `git --version` in Terminal again to confirm. You should see a version number. ✅

---

### 🔧 Step 3: Tell Git Who You Are

Git needs to know your name and email so it can label your work correctly. This only needs to be done once per computer.

**This step is the same on Windows (Command Prompt) or Mac (Terminal):**

1. Open your terminal (Command Prompt on Windows, Terminal on Mac— same as above).
2. Type the following, replacing `Your Name` with your actual name, and press **Enter**:
   ```
   git config --global user.name "Your Name"
   ```
3. Now type the following, replacing the fake email below with the one you used for your GitHub account, and press **Enter**:
   ```
   git config --global user.email "youremail@example.com"
   ```
4. To confirm it worked, type the following and press **Enter**:
   ```
   git config --global --list
   ```
   You should see your name and email listed. ✅

📖 Learn more: [Setting your username in Git](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)

---

### 🔧 Step 4: Install GitHub Desktop

GitHub Desktop is a visual application that lets you manage your Git repositories without needing to memorize command line instructions.

**📌 Windows and Mac:**

1. Go to [https://desktop.github.com/](https://desktop.github.com/)
2. Click the **Download** button. The site will automatically detect your operating system.
3. Open the downloaded file and follow the installation prompts.
4. GitHub Desktop will open automatically when installation is complete.

📖 Learn more: [Installing GitHub Desktop](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/installing-github-desktop)

---

### 🔧 Step 5: Sign Into GitHub Desktop

Now you'll connect GitHub Desktop to your GitHub account (this is called "authenticating").

**📌 Mac:**
1. In the top menu bar, click **GitHub Desktop**, then click **Settings**.
2. In the Settings window, click the **Accounts** tab on the left.
3. Click the **Sign Into GitHub.com** button.
4. A browser window will open — follow the prompts to log in with your GitHub username and password.
5. Once done, your name should appear in the Accounts tab. ✅

**📌 Windows:**
1. In the top menu bar, click **File**, then click **Options**.
2. In the Options window, click the **Accounts** tab on the left.
3. Click the **Sign Into GitHub.com** button.
4. A browser window will open — follow the prompts to log in with your GitHub username and password.
5. Once done, your name should appear in the Accounts tab. ✅

📖 Learn more: [Authenticating to GitHub in GitHub Desktop](https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/authenticating-to-github-in-github-desktop)

**Connect VS Code to GitHub Desktop:**
1. Open **GitHub Desktop**.
2. **On Mac:** Click **GitHub Desktop** in the top menu bar, then **Settings**. Click the **Integrations** tab. Under "External Editor," select **Visual Studio Code** from the dropdown.
3. **On Windows:** Click **File** in the top menu bar, then **Options**. Click the **Integrations** tab. Under "External Editor," select **Visual Studio Code** from the dropdown.
4. Click **Save**. ✅

Now when you open a repo in GitHub Desktop, you can launch VS Code directly from it!

---

## Part 2: Keeping Your Repos Organized

Before you start creating files everywhere, let's talk about organization. This is a habit worth building from day one. The best way to keep your thoughts organized is to keep your workspace organized. You'll want to make sure any local repos you create are in the same location and not scattered all over your machine.

### 📁 Create a dedicated folder for all your GitHub projects

Pick one place on your computer where ALL your GitHub repositories will live. I try to keep mine as close to the root as I'm comfortable with to ensure smaller paths to projects in the future. Good options:

- `Documents/GitHub/`
- `Desktop/GitHub/` *(not recommended long-term — your Desktop gets cluttered fast!)*
- `Users/Username/GitHub`


**To create this folder:**

- **Windows:** Open File Explorer, navigate to your Documents folder, right-click in the empty space, select **New > Folder**, and name it `GitHub`.
- **Mac:** Open Finder, navigate to your Documents folder, press `Shift + Command + N` to create a new folder, and name it `GitHub`.

> 💡 **Best Practice:** Always clone and create repos inside this one folder. When you have 20+ repos someday, you'll be very glad you did this!

---

## Part 3: Create a Local Repository and Push It to GitHub

Now that everything is installed, let's get to work on using GitHub locally. 

### Step 1: Create a New Repository in GitHub Desktop

1. Open **GitHub Desktop**.
2. In the top menu bar, click **File**, then click **New Repository...** (on Mac this might also appear as `New Repository...` in the GitHub Desktop menu).
3. A dialog box will appear. Fill it in:
   - **Name:** `my-local-repo` *(or any name you like — no spaces! Use hyphens instead)*
   - **Description:** `My first locally created repository` *(optional, but good habit)*
   - **Local Path:** Click **Choose...** and navigate to the `GitHub` folder you created in Part 2. Select it and click **Choose**.
   - **Initialize this repository with a README:** ✅ Check this box.
   - Leave all other options as their defaults.
4. Click **Create Repository**.

You've just created a real Git repository on your computer! 🎉

> 📄 **What's `.gitattributes`?** GitHub Desktop automatically creates a file called `.gitattributes` in your new repo. This file tells Git how to handle line endings — the invisible characters that mark the end of a line in a text file. Different operating systems use different line ending styles (Windows uses `CRLF`, Mac/Linux use `LF`), which can cause problems when collaborators on different systems edit the same files. The `.gitattributes` file normalizes this automatically so everyone stays in sync. You don't need to edit it — just leave it as-is!

### Step 2: Open It in VS Code

1. In GitHub Desktop, you should now see your new repository loaded in the main window.
2. Click the button that says **Open in Visual Studio Code** (it may show up in the center of the screen or you may have to find it manually under the **Repository** menu at the top). This will open your project folder in VS Code.

### Step 3: Make a Change to the README
> ⚠️ Hey, what's the first thing you should do before making changes in a repo? That's right! MAKE A NEW BRANCH! In this case, we're going to commit right to main for this, and then make a branch later. Yes, this isn't best practice for any changes, but you've got special permission this one time to commit right to main. 🎉

1. In VS Code, look at the left-hand panel (called the **Explorer**). You should see a file called `README.md`. Click on it.
2. The file will open in the main editor area. You'll see some default text.
3. Click at the end of the text and add a new line. Type something like:
   ```
   This repository was created locally on my computer!
   ```
4. Save the file by pressing `Ctrl + S` on Windows or `Command + S` on Mac.
     - This is a big difference between working locally and in a browser in [GitHub Codespaces](https://docs.github.com/en/codespaces) or the GitHub Web Editor. In those browser based IDEs, your work gets autosaved. When working locally, you need to actually save your files first. This can trip up a lot of new developers, and it even messes me up sometimes when I'm working locally wondering why my changes aren't showing up. So make sure to remember this step of saving when working in VSCode. 

### Step 4: Commit Your Changes in GitHub Desktop

1. Switch back to **GitHub Desktop**.
2. You'll notice the left panel now shows your changed file (`README.md`) with checkmarks next to it. This means GitHub Desktop has detected your changes!
3. At the bottom left of the screen, there is a box labeled **Summary (required)**. Type a short description of what you did, for example:
   ```
   Add personal note to README
   ```
   > 💡 **Best Practice:** Commit messages should be short and descriptive. Imagine someone else (or your future self) reading it — will they understand what changed? "Updated stuff" is bad. "Add personal note to README" is good.
4. Click the blue **Commit to main** button.

You've made your first local commit! ✅

### Step 5: Publish (Push) Your Repository to GitHub

Your repo only exists on your computer right now. Let's push it to GitHub so it lives online too.

1. Once you click **Commit to main**, you'll be taken to a new screen that says "No local changes". Since it recognizes that your repo isn't on GitHub yet, There's a big blue button to publish it. There's another button near the top of the app as well that says **Publish repository**. Click one or the other.
2. A dialog will appear:
   - **Name:** Leave as-is.
   - **Description:** Optionally add a description.
   - **Keep this code private:** Uncheck this if you want it to be public, or leave it checked to keep it private. Either is fine for this exercise.
   - **Organization** Likely not there, but if it is, choose `None`
3. Click **Publish Repository**.
4. Open your browser and go to [https://github.com](https://github.com). Click on your profile icon in the top right and click **Your repositories**. You should now see `my-local-repo` in the list! ✅

---

## Part 4: Create a New Branch Locally and Push It

As you know, branches let you work on changes without affecting the main version of your project. This is one of the most important GitHub concepts. You've made new branches in the Web editor before, now it's time to do it in GitHub Desktop! 

### Step 1: Create a New Branch in GitHub Desktop

1. In GitHub Desktop, look at the top of the screen. You'll see three sections in the top bar: your current repository name, the current branch name (it says **main**), and a push or fetch button.
2. Click on the box that says **main** (the current branch). A dropdown will appear.
3. Click **New Branch**.
4. In the box that appears, type a name for your branch:
   ```
   my-first-gh-desktop-branch
   ```
5. Click **Create Branch**.

You're now on your new branch! Notice the branch selector at the top now shows your new branch name instead of "main." ✅

### Step 2: Make a Change on Your Branch

1. Click **Open in Visual Studio Code** in GitHub Desktop (somewhere in the middle).
2. In VS Code, you should be able to see that you're working on a new branch by looking at the bottom left. Your branch name `my-first-gh-desktop-branch` (or whatever you chose) should be there. 
3. Click the **README.md** file in the Explorer panel on the left.
4. Add another new line at the bottom:
   ```
   I made this change on a branch!
   ```
5. Save the file with `Ctrl + S` (Windows) or `Command + S` (Mac).

### Step 3: Commit the Change

1. Switch back to **GitHub Desktop**.
2. You'll see the README.md file listed as changed.
3. In the **Summary** box at the bottom left, type:
   ```
   Add branch note to README
   ```
4. Click **Commit to [your-branch-name]**.

### Step 4: Push Your Branch to GitHub

1. At the top of GitHub Desktop, you'll now see a button that says **Publish branch**. Click it.
2. Your branch is now on GitHub! ✅

**To verify:** Go to your repository on GitHub.com (`github.com/your-username/my-local-repo`). Click the branch dropdown (it shows "main" by default, near the top left of the file list). You should see your new branch in the list!



---

## Part 5: Make a Change on GitHub and Pull It Locally

So far you've been making changes locally and pushing them up to GitHub. But what about the other direction? When a change is made directly on GitHub.com — by you or a collaborator — you need to **pull** those changes down to your local machine to stay in sync.

### Step 1: Make a Change on GitHub.com

1. Open your browser and go to [https://github.com](https://github.com).
2. Navigate to your `my-local-repo` repository.
3. Click on the `README.md` file to open it.
4. Click the **pencil icon** (Edit this file) in the top right of the file view.
5. Add a new line at the bottom of the file, for example:
   ```
   This change was made directly on GitHub.com!
   ```
6. Scroll down to the **Commit changes** section. Add a short commit message like:
   ```
   Add note from GitHub.com editor
   ```
7. Make sure **Commit directly to the `main` branch** is selected (lots of committing to main happening here...), then click **Commit changes**.

Your change is now on GitHub, but your local copy doesn't know about it yet.

### Step 2: Pull the Change in GitHub Desktop

1. Open **GitHub Desktop**.
2. Make sure you're on the `main` branch (check the branch selector at the top — click it and select **main** if needed).
3. At the top of the screen, you'll see a button that says **Fetch origin**. Click it. GitHub Desktop will check for any new changes on GitHub.
4. The button will update to say **Pull origin** with a small number indicating there's 1 new commit. Click **Pull origin**.

GitHub Desktop will download the change and your local `README.md` now matches what's on GitHub.com. ✅

### Step 3: Verify in VS Code

1. Click **Open in Visual Studio Code** in GitHub Desktop.
2. Open `README.md` in the Explorer panel — you should see the line you added on GitHub.com is now there locally.

> 💡 **Best Practice:** Get into the habit of clicking **Fetch origin** at the start of every work session. It checks for any changes made elsewhere and lets you pull them before you start editing — preventing [merge conflicts](/merge_conflict/) down the road.

---

## Part 6: Clone Your Profile README

Now you'll clone a repository that **already exists on GitHub** (your Profile README) to your local computer. Cloning means making a copy of an online repo on your machine.

> NOTE: This whole section is using your profile readme, a repository you created on github.com. This work assumes you haven't pulled the work locally yet and that the repo only exists on your remote repo (github.com/yourusername/yourusername). If you've already cloned the repo locally, then you likely don't need this section anyway! 

### Step 1: Find Your Profile README on GitHub

1. Open your browser and go to [https://github.com](https://github.com).
2. Click your profile icon in the top right corner, then click **Your repositories**.
3. Find the repository named after your GitHub username (e.g., if your username is `octocat`, look for a repo called `octocat`). This is your Profile README.
4. Click on the repository to open it.

### Step 2: Clone It Using GitHub Desktop

**Method 1 - Directly from GitHub.com (Easiest):**
1. On your repository page, click the green **<> Code** button near the top right of the file list.
2. In the dropdown that appears, click **Open with GitHub Desktop**.
3. GitHub Desktop will open and show a "Clone a Repository" dialog.
4. Click **Choose...** next to the Local Path field, and navigate to your `GitHub` folder from Part 2.
5. Click **Clone**.

**Method 2 - From inside GitHub Desktop:**
1. In GitHub Desktop, click **File** in the top menu, then click **Clone Repository...**
2. Click the **GitHub.com** tab. You'll see a list of your repositories.
3. Find and click on your Profile README repository (the one named after your username).
4. Click **Choose...** next to the Local Path and navigate to your `GitHub` folder.
5. Click **Clone**.

GitHub Desktop will download the repository to your computer. Once done, you'll see it loaded in GitHub Desktop. ✅

### Step 3: Open It and Explore

1. Click **Open in Visual Studio Code** in GitHub Desktop.
2. You'll see your Profile README files in VS Code's Explorer panel on the left.
3. Try opening `README.md` and making a small change (like fixing a typo or adding a line).
4. Save the file, switch to GitHub Desktop, write a commit message, and click **Commit to main**. (Again, VERY SPECIAL INSTRUCTIONS where it's ok to commit to main 😃)
5. Click **Push origin** (the button at the top of GitHub Desktop) to push your change to GitHub.
6. Go to your GitHub profile page to see your change live! 🎉

📖 Learn more: [Cloning a repository from GitHub to GitHub Desktop](https://docs.github.com/en/desktop/adding-and-cloning-repositories/cloning-and-forking-repositories-from-github-desktop)

---

## ⚠️ Common Mistakes and How to Fix Them

### ❌ "I can't find the 'Open with GitHub Desktop' button on GitHub.com"
**Fix:** Make sure GitHub Desktop is fully installed and that you've opened it at least once before trying to use this button. Some browsers may also ask you to confirm opening the external application — click **Allow** or **Open GitHub Desktop** when prompted.

---

### ❌ "I forgot to select my GitHub folder as the location — my repo was saved somewhere random"
**Fix:** Don't panic! In GitHub Desktop, click **File > Add Local Repository...**, then navigate to wherever the repo was saved and select it. For next time: always pay attention to the **Local Path** when creating or cloning repos.

---

### ❌ "I committed to `main` instead of my branch"
**Fix:** This happens! For small personal projects it's often fine. If you need to undo a commit, in GitHub Desktop go to **History** (in the left panel), right-click the most recent commit, and select **Undo Commit**. Your changes will come back as uncommitted. Then switch to your branch first and recommit.

---

### ❌ "GitHub Desktop says 'Authentication failed' when I try to push"
**Fix:** You may need to sign in again. In GitHub Desktop, go to **File > Options** (Windows) or **GitHub Desktop > Settings** (Mac), click **Accounts**, sign out, and sign back in. If the problem persists, check your internet connection.

---

### ❌ "I pushed my branch but I can't find it on GitHub.com"
**Fix:** Make sure you clicked **Publish Branch** in GitHub Desktop (not just committed). Also double-check you're looking at the right repository on GitHub.com. Click the branch dropdown on the repo page — it should be in the list.

---

### ❌ "VS Code isn't showing up as an option in GitHub Desktop's Integrations"
**Fix:** Make sure VS Code finished installing completely. Try restarting GitHub Desktop after installing VS Code. On Mac, also make sure VS Code is in your `Applications` folder.

---

### ❌ "My terminal says 'git is not recognized' on Windows"
**Fix:** Git may not have been added to your system's PATH during installation. The easiest fix is to uninstall Git and reinstall it, making sure to leave the default options as-is during setup (the installer handles PATH automatically with default settings).

---

## 💡 Best Practices

- **Always check which branch you're on before making changes.** In GitHub Desktop, the current branch is always shown at the top. Get in the habit of glancing at it before you open VS Code.
- **Commit often.** Small, frequent commits are better than one giant commit at the end. It makes it much easier to understand the history of a project.
- **Always write meaningful commit messages.** `"Fix typo in bio section"` is infinitely more useful than `"changes"`.
- **Use the web editor (press `.` in any repo on GitHub.com) for quick text edits** — no need to open a full Codespace or switch to your local setup for small fixes like typos.
- **Pull before you push.** If you're working on a project that others might be changing too (or that you've changed on another computer), click **Fetch origin** in GitHub Desktop first to download the latest changes before you start working.
- **Keep your GitHub folder clean.** Only clone repos you're actively working on. You can always re-clone something later if you delete your local copy — the GitHub.com version is always there.
- **Keep GitHub Desktop updated.** It will often notify you of updates. Install them — they often include bug fixes and usability improvements.

---

## 📚 Additional Resources

- [About GitHub Desktop](https://docs.github.com/en/desktop/overview/about-github-desktop)
- [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/overview/getting-started-with-github-desktop)
- [Managing branches in GitHub Desktop](https://docs.github.com/en/desktop/making-changes-in-a-branch/managing-branches-in-github-desktop)
- [Connecting to GitHub — Working from the desktop](https://docs.github.com/en/get-started/using-github/connecting-to-github#working-from-the-desktop)
- [Setting your username in Git](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)
- [VS Code Download](https://code.visualstudio.com/)

---

**🎉 Congratulations!** You've set up a full local GitHub workflow. You installed the tools, connected them to GitHub, created a repo from scratch on your computer, worked with branches, and cloned an existing repo. This is the exact same workflow professional developers use every day!