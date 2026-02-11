---
layout: default
title: Collaborative Activity
nav_order: 3
permalink: /collaborative/
---


# Lesson Plan: Collaborating in a Group on GitHub (3–4 People)

In this activity, a group of 3–4 learners will work **together in one GitHub repository**.  
Each person will:

- Create **their own branch**.  
- Add **their own Markdown file**.  
- Open **their own pull request (PR)** into the `main` branch.  
- Merge without causing any merge conflicts.

This activity follows GitHub’s shared repository workflow, where collaborators create branches in one repository and use pull requests to propose and review changes. 
---

## 1\. Prerequisites

Learners should:

- Have a **GitHub account** (Free or Pro).  
- Be able to **sign in** to GitHub at least.  
- Have a **web browser** (Chrome, Edge, Firefox, Safari).  
- Have been added as **collaborators** to a shared practice repository (the instructor can own this repository).

Helpful GitHub docs:

- About branches ([docs.github.com](https://docs.github.com/enterprise-cloud%40latest/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests?utm_source=openai))  
- About pull requests ([docs.github.com](https://docs.github.com/en/enterprise-server%403.16/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests?utm_source=openai))

[Example Repo](https://github.com/MetzinAround/our-collab-practice) 

---

## 2\. Learning Goals

By the end of this activity, learners will be able to:

1. Explain why teams use **branches** when working together.  
2. Create a **personal branch** in a shared repository.  
3. Create and edit a **Markdown file** in the GitHub web editor.  
4. Open a **pull request** from their branch into `main`.  
5. Review and **merge** pull requests one-by-one **without merge conflicts**, by:  
   - Keeping each file unique per person.  
   - Waiting for each PR to finish merging before starting another if they touch the same place.

---

## 3\. Instructions for Learners

### Part A – Creating and Sharing the Repository

1. **Person 1: Create a repository**:  
     
   - Sign in to GitHub.  
   - In the upper-right corner, click your profile picture.  
   - Click **“Your repositories”**.  
   - Click the green **“New”** button.  
   - Give the repository a name: `our-collab-practice`.  
   - Select **Private**   
   - Check **“Add a README file”**.  
   - Click **“Create repository”**.  
       
2. **Person 1: Add learners as collaborators**:  
     
   - On the repository page, click the **“Settings”** tab.  
   - In the left sidebar, click **“Collaborators”**.  
   - Click **“Add people”**.  
   - Type each group member’s GitHub username and invite them.  
   - Learners must accept the email or web invitation before they can push changes.  
       
3. **Persons 2- 4: Accept the invitation**  
     
   - Open your email or GitHub notifications.  
   - Click on the invitation to join the repository.  
   - Click **“Accept invitation”**.

---

### Part B – Open Web Editor and Create Your Personal Branch (Persons 1 \- 4\)

You will create a branch that only you use.

1. **Open the web editor (github.dev)**  
   - On your repository’s main page, press the **`.` (period)** key on your keyboard.  
   - A new tab opens showing a VS Code–like editor in your browser.  
   - If asked, sign in again and authorize.

2. **Create a new branch**  
     
   - Look at the **bottom-left corner** of the web editor. You’ll see the current branch name (usually `main`).  
   - Click the branch name.  
   - In the small box that appears at the top, click **“Create new branch…”**.  
   - In the text box that appears, **type your branch name**. Use this pattern:

   

     - `yourname-branch`, for example:  
       - `cindy-branch`  
       - `horton-branch`  
       - `martha-branch`  
   - Press **Enter**.  
   - At the bottom-left, confirm it now shows your **new branch name** instead of `main`.

You have now created your own branch, all work will be done on this branch unless otherwise indicated. 

---

### Part C – Create Your Personal Markdown File (Persons 1 \- 4\)

To avoid merge conflicts, each person will create a **different file name**.

#### 1\. Make sure you are on your branch

1. Look at the **bottom-left corner** of the web editor.  
2. You should see your branch name there, for example: `cindy-branch`.  
3. If it says `main` or something else:  
   - Click the branch name at the bottom-left.  
   - A box appears at the top of the page with a list of branches.  
   - Click **your branch name** (for example, `cindy-branch`).  
   - Check again at the bottom-left to confirm it now shows **your branch**.

#### 2\. Create a new file

1. In the **Explorer** panel on the left (the list of files), move your mouse into the empty space under the last file.  
2. Right-click in that space and choose **“New File”**  
   - ALTERNATE NEW FILE CREATION: There is a small icon that looks like a page with a plus sign on it. This will create a new file as well. Notice the other icons to the right of the circled one below. They are for creating new folders/directories, refreshing the file explorer, and collapsing all directories. 

   ![image](/assets/explorer%20icon.png)

#### 3\. Name the file

1. A small text box appears for the file name.  
2. Type a unique file name using this pattern: `yourname.md`  
   Examples:  
   - `cindy.md`  
   - `horton.md`  
   - `martha.md`  
3. Press **Enter** on your keyboard.  
   Make sure **no two people use the same name**.

#### 4\. Write some content in Markdown

1. After you press Enter, a blank editor opens for your new file.  
     
2. Click inside the large editing area and type something like this (you can change it):

```
1 # About Cindy
2
3 - School you teach at
4 - Favorite "wake up" beverage
5
```

3. NOTE: the numbers are the line numbers. Do not type the numbers.   
4. Replace the word **“Cindy”** and the bullet points with **your own** information.

#### 5\. Save (commit) the new file to your branch

1. In the web editor, look at the **left sidebar** and click the **Source Control** icon, circled in the picture below.

![image](/assets/giticon.png)

2. At the top of the Source Control panel, you will see a box labeled **“Message”**.  
3. Click in that box and type a short commit message, for example:  
   `Add cindy profile file`  
4. Below the message box, click the **“+” (plus)** icon next to **“Changes”** or next to your new file name to stage it.  
5. After staging, click the checkmark icon **“Commit”** above the message box.  
6. A small message may appear asking if you want to stage and commit all changes; if it does, click **“Yes”**.

Your file is now **saved (committed) on your personal branch**, but it is **not in `main` yet**.

---

### Part D – Check That Everyone’s Work Is Separate (Persons 1 \- 4\)

As a group, quickly confirm:

1. Everyone has a **different branch name**, for example:  
   - `cindy-branch`  
   - `horton-branch`  
   - `martha-branch`  
2. Everyone has a **different file name**, for example:  
   - `cindy.md`  
   - `horton.md`  
   - `martha.md`  
3. No one edited the same existing file (such as `README.md`).

Because each person works in a **different file on their own branch**, Git will be able to merge all pull requests into `main` **without merge conflicts**.

---

### Part E – Open a Pull Request (PR) for Your Branch (Persons 1 \- 4\)

Now you will propose to merge your branch into `main` using a pull request.

1. Make sure you are on **the repository page.**   
     
   - At the top-left branch dropdown, confirm it shows your branch name (for example, `cindy-branch`).

   

2. Open the **“Compare & pull request”** page:  
     
   - You might see a yellow bar near the top saying something like:  
     - “`cindy-branch` had recent pushes less than a minute ago” with a **“Compare & pull request”** button.  
   - If you see this button, click **“Compare & pull request”**.

   

   If you **do not** see the yellow bar:

   

   - Click the **“Pull requests”** tab near the top of the repository page.  
   - Click the green **“New pull request”** button.  
   - On the left side (base), make sure it says:  
     - **base: `main`**  
   - On the right side (compare), open the dropdown and select **your branch name**, for example `cindy-branch`.

   

3. Fill out the pull request form:  
     
   - At the top, in the **Title** box, type a short title, for example:  
     - `Add cindy profile markdown file`  
   - In the larger **Description** box, type a couple of sentences explaining the Pull Request.  
     

REMEMBER: A typical Pull Request should include why the PR is being requested (“Don’t just say what, say why”), but for these assignments there’s no need for long descriptions. 

4. Confirm which branches are involved:  
     
   - Near the top, it should say something like:  
     - `base: main` ← `compare: cindy-branch`  
   - This means you are asking to merge **from your branch** into **main**.

   

5. Create the pull request:  
     
   - Click the green **“Create pull request”** button.

You have now opened a PR from your branch into `main`.

---

### Part F – Review Each Other’s Pull Requests (Persons 1 \- 4\)

At this point, you should be able to see everyone’s branches on the main page of the repo and everyone’s PRs. 


![image](/assets/branches.png) 

![image](/assets/pullrequests.png)

Each group member should review at least one other member’s PR.

1. Go to the **“Pull requests”** tab at the top of the repository.  
2. You will see a list of all open pull requests from your teammates.  
3. Each member of the group should review one other teammate’s PR.  
4. On the pull request page:  
   - Read the **Title** and **Description**.  
   - Click the **“Files changed”** tab.  
   - Scroll to see their Markdown file, for example `horton.md`.  
5. Add a simple comment:  
   - At the top of the pull request, click in the **“Leave a comment”** box (or click specific line numbers in the file view and click the blue **“+”** to comment on a line).  
   - Add a comment.   
   - Click **“Comment”**.  
6. While still in the files changed tab, click `Review Changes` to the right of the window.   
7. Add a comment to the comment box and click `Approve`

---

### Part G – Merge Pull Requests Without Conflicts (Person 1\)

Because each person created a **different file**, GitHub can merge all pull requests cleanly.

Choose the owner of the Repo to act as the **merger**.  
They will merge each PR one at a time.

For each pull request:

1. Go to the **“Pull requests”** tab.  
2. Click one open PR.  
3. Scroll down to the bottom of the Conversation tab.  
4. If everything looks good, click the green **“Merge pull request”** button.  
5. In the box that opens, click **“Confirm merge”**.  
6. Repeat for each team member’s PR.

---

### Part H – Verify That Everyone’s Files Are in `main`

After all PRs are merged:

1. At the top-left branch dropdown, choose **`main`**.  
     
2. On the main repository page, look at the file list.  
     
3. You should see **all Markdown files**, one for each person:  
     
   - `cindy.md`  
   - `horton.md`  
   - `martha.md`  
   - (and so on)

   

4. Click each file to open it and confirm that the content is correct.

---

## 6\. Reflection / Discussion Questions

Discuss these as a group or write answers in your Markdown file:

1. Why did we create **separate branches** instead of editing `main` directly?  
2. How did having **one file per person** prevent merge conflicts?  
3. Where in GitHub did you see information about what changed in a pull request?  
4. How could this workflow scale to a larger project with many files?

---

## 7\. Best Practices and Tips

These are not strictly required to complete the activity, but they will help you as you continue to use GitHub.

1. **One branch per task or person**  
     
   - Use a separate branch for each feature or person.  
   - This keeps work organized and makes it easier to review.

   

2. **Use descriptive branch names**  
     
   - Instead of `test1`, use:  
     - `cindy-profile-page`  
     - `horton-update-readme`  
   - This helps teammates understand what each branch is for. ([worldbank.github.io](https://worldbank.github.io/template/docs/git-workflows.html?utm_source=openai))

   

3. **Keep branches up to date**  
     
   - On larger projects, if `main` changes often, you may need to update your branch from `main` before opening or merging a PR. (For this simple activity, we avoided conflicts by editing different files.)

   

4. **Clear pull request titles and descriptions**  
     
   - Write titles that describe what the PR does:  
     - “Add cindy profile markdown file” is better than “Update stuff”.  
   - In the description, explain **why** you made the change, not just what you did.

   

5. **Review before merging**  
     
   - Even simple changes should be quickly reviewed by a teammate.  
   - Look for:  
     - Typos.  
     - Missing information.  
     - Anything confusing.

   

6. **Use the web editor for simple changes**  
     
   - For quick edits like this activity, you can stay entirely in the **GitHub web interface**:  
     - Use **“Add file → Create new file”** and **“Edit this file”** buttons.  
   - You do **not** need to set up Git on your computer for basic practice.

   

7. **One PR should not touch too many unrelated things**  
     
   - Try to keep each PR focused on a small, clear goal (for example, “Add my profile file”).  
   - This makes reviewing easier and reduces conflicts.

---

## 8\. Extension Ideas (Optional)

If your group finishes early, try one or more of these:

1. **Edit an existing shared file without conflicts**  
     
   - As a group, open `README.md`.  
   - Decide on **different sections** for each person (for example, each person adds their name in a different bullet list).  
   - Each person:  
     - Creates a new branch.  
     - Edits a different part of the README.  
     - Opens a PR.  
   - Discuss what would happen if two people tried to edit **the same line**.

   

2. **Assign reviewers**  
     
   - When creating a PR, use the **“Reviewers”** section on the right side to request a review from a specific teammate.

   

3. **Practice closing a PR without merging**  
     
   - Create a tiny change on a branch.  
   - Open a PR.  
   - Then click **“Close pull request”** instead of merging.  
   - Observe that the branch is still there, but the change is not in `main`.

---

Learners who complete this activity should feel comfortable with the **basic collaborative GitHub workflow**: branches, Markdown files, pull requests, review, and merge—while also understanding how to avoid merge conflicts by organizing work clearly.