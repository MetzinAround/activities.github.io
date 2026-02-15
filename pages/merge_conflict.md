---
layout: default
title: Creating and Solving a Merge Conflict
nav_order: 4
permalink: /merge_conflict/
---

# Creating and Solving a Merge Conflict
*A beginner-friendly GitHub collaboration activity (groups of 3 - 4)*

GitHub exists to make collaboration easier. In this activity, you’ll practice a real team workflow: adding collaborators, making branches, opening pull requests, and intentionally resolving a merge conflict.

---

## Recommended documentation (reference links)
- Adding collaborators: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-access-to-your-repository
- About branches: https://docs.github.com/en/get-started/using-git/about-branches
- About pull requests: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests
- About merge conflicts: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts

---

## Group setup
Form **groups of three - 4 **:
- **1 Repo Owner (Lead)**
- **2 - 3 Collaborators**

All pull requests will be made **into the Repo Owner’s repository**.

---

## Part A — Repo Owner: Create the repository and add collaborators

### Create a new repository (Repo Owner)
1. Go to https://github.com and make sure you’re signed in.
2. In the top-right corner, click the **+** icon. It is a few icons to the left of your profile picture.
3. Click **New repository**.
4. For **Repository name**, type: `Paired work`
5. Set **Visibility** to **Public**.
6. Check the box for **Add a README file**.
7. Click **Create repository**.

### Add the other two people as collaborators (Repo Owner)
1. Inside your new repository, click the **Settings** tab.
2. On the left sidebar, click **Collaborators** (sometimes it appears under “Access” / “Collaborators and teams” depending on UI).
3. Click **Add people**.
4. Type the first collaborator’s GitHub username (example: `MarthaMayWhovier`).
5. Select the correct user from the dropdown.
6. Click **Add USERNAME to this repository**.
7. Repeat for the second collaborator.
8. Learners must accept the email or web invitation (in notifications near the top right of each page) before they can push changes.

---

## Part B — Collaborators: Accept the invitation (All non-owners)

Each collaborator must accept the invite before they can push branches.

1. Go to https://github.com/notifications
2. Look for a repository invitation.
3. Click **View invitation** (or open the invitation notification).
4. Click **Accept invitation**.

If you don’t see it:
- Ask the Repo Owner to confirm they entered the correct username.
- Refresh the page.
- Check email tied to your GitHub account (sometimes GitHub emails repo invites).
- Navigate directly to the repo and a banner should appear saying you've been invited. 

---

## Part C — Repo Owner: Create the “conflict bait” file on `main`

The Repo Owner will add a file directly to the `main` branch (this is intentional for the exercise).

### Open the GitHub web editor
1. Go to the main page of your repository (click the **Code** tab if needed).
2. Press the **period key** on your keyboard: `.`
   - This opens the GitHub web editor (looks similar to VS Code in the browser).

> Tip: If pressing `.` doesn’t work, make sure you clicked somewhere on the page first, and that your cursor isn’t inside a text field. You can also navigate to it by replacing the `com` in your repo url with `dev`. 
    - https://www.github.com/besteechur/paired_work is the url for the GitHub repo
    - https://www.github.dev/besteechur/paired_work is the url for the web editor

### Create a new file named `lets_make_a_conflict.md`
1. In the left file sidebar, look for an option like **New File** (or use the file explorer menu).
2. Name the file, `lets_make_a_conflict.md`
3. Paste or type the following template into the file (including blank lines):

```
YOUR_NAME_HERE
YOUR_FAVORITE_FOOD_HERE

YOUR_FAVORITE_TV_SHOW_OR_MOVIE_HERE
```
Make sure the third line is left blank.

### Commit directly to `main`
1. Find the **Source Control** icon on the left sidebar (it usually looks like a branching icon).
2. You should see your new file listed under **Changes**.
3. Next to **Changes**, click the **+** to stage the change (if staging is shown).
4. In the message box, type a commit message like:  
   `Add conflict practice file`
5. Click **Commit & Push** (or **Commit changes**).
6. You've now committed directly to main! YOU NORMALLY WOULDN'T COMMIT TO MAIN. 
---

## Part D — Collaborators: “The One Change PR” (All non-owners)

Both collaborators will:
- Open the web editor
- Create a branch
- Add their info to the same file (to create future conflict conditions)
- Commit & push
- Open a Pull Request into `main`

### Open the repository and launch the web editor
1. Go to the Repo Owner’s repository page in your browser.
2. Press the **period** key: `.` to open the web editor.

### Create your own branch
1. In the web editor, look at the bottom-left corner for the current branch name (it will usually say **main**).
2. Click **main**.
3. Choose **Create new branch…**
4. Name it using your username in this format:
   - `username-edits`  
   Example: `BestTeeChur-edits`
5. Confirm/create the branch.

You should now see your branch name in the bottom-left instead of `main`.

### Edit the file (do not delete or replace — only add to it)
1. In the file list, click `lets_make_a_conflict.md`.
2. Add your info starting on **line 5** (below the Repo Owner’s entry). Do not remove what’s already there.
3. Format it like this:

- **Line 5**: your name  
- **Line 6**: your favorite food  
- **Line 7**: blank line  
- **Line 8**: your favorite TV show or movie  

So the file should look like two “blocks” of info, one after the other, with a blank line separating them.

### Commit & push your changes
1. Click the **Source Control** icon on the left sidebar.
2. Under **Changes**, click the **+** to stage all changes.
3. In the message box, type a commit message like:  
   `Add my info to conflict file`
4. Click **Commit & Push**.

### Open a Pull Request (PR) to `main`
1. Go back to the repository page in your browser tab (the normal GitHub page, not the editor).
   - Click the bottom left button that says "GitHub". It will open a menu from up top and you can click "Go to Repository. You can also click the back button from the web editor until you arrive. You can also open a whole new tab and manually go to your repository.
2. Refresh the page (press **F5** or use the browser refresh button).
3. Click the **Pull requests** tab.
4. Click the green **New pull request** button.
5. Set the branches:
   - **Base**: `main`
   - **Compare**: your branch (example: `BestTeeChur-edits`)
6. Add a title like:  
   `Add BestTeeChur's info`
7. In the description, write:
   - What you changed (added your info)
   - Why (workshop collaboration practice)
8. **Assign the PR to the Repo Owner**:
   - On the right sidebar, find **Assignees**
   - Click **Assignees**
   - Select the Repo Owner
9. Click **Create pull request**.

---

## Part E — Repo Owner: Merge ONLY ONE PR
This is after both Pull Requests have been made

1. Go to the **Pull requests** tab in your repo.
2. Open one of the submitted PRs.
3. Scroll down and click the green **Merge pull request** button.
4. Confirm the merge.

Important: **Do not merge the second PR yet.** That PR will now produce a merge conflict.

---

## Part F — The merge conflict: Resolve the second PR (Repo Owner + group discussion)

### What is a merge conflict (plain language)?
A merge conflict happens when GitHub sees changes that don’t “fit together” automatically—usually because **two branches changed the same lines** in different ways. GitHub pauses the merge so a human can decide what the final file should look like.

### Open the remaining PR that was NOT merged
1. In the repo, go to the **Pull requests** tab.
2. Click the PR that is still open (the one from the third group member).
3. You should see that it **can’t be merged automatically**.
   - The merge button will be disabled/gray.
4. Click **Resolve conflicts** (or follow the prompt GitHub provides).

### Edit the conflict markers until the file looks correct
GitHub will show a conflict editor with special markers like:

- `<<<<<<<`
- `=======`
- `>>>>>>>`

Your job: remove the markers and make the file look how you want the final version to look.

**Goal for this exercise:** the final file should include **all group members'**:
- name
- favorite food
- (blank line)
- favorite TV show/movie

…and each person’s “block” should be on separate lines, readable, and not overwriting anyone else.

### Mark resolved and complete the merge
1. When the file looks correct, click **Mark as resolved** (if shown).
2. Click **Commit merge** (or the button GitHub shows to finalize).
3. After that commit, click **Merge pull request** (GitHub will now allow it).
4. Confirm the merge.

---

## Best practices (helpful tips, not required)
- **Use branches for all changes** (even small ones) in real teamwork. Committing to `main` directly is usually avoided outside of controlled exercises.
- **Write descriptive commit messages** (e.g., “Add workshop participant info”).
- **Keep PRs small and focused** (“one change PR” is great practice).
- **Communicate before editing the same lines** to reduce conflicts (or intentionally coordinate when conflicts are expected).
- **Use the web editor for quick edits**:
  - Press `.` on a repo page to open it quickly in the browser editor.