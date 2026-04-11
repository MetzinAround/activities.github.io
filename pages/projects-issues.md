---
layout: default
title: Using Issues and Projects
nav_order: 4
permalink: /projects-issues/
---

# Using GitHub Projects & Issues to Stay Organized

A great way to stay on top of any project is to use GitHub Issues and Projects. Issues let you track individual tasks, and Projects give you a visual board to see everything at once — just like a real development team would use!

In this lesson, you'll set up a mock school project **on your own**, playing the role of a project manager organizing tasks for a team. Even though you're working solo, everything you set up here is exactly how a real team would use it — so when it's time to collaborate, you'll already know the ropes.

>NOTE: We're using four fictional names to represent partners in this project: Martha, Cindy, Horton, and Ted. While you can't assign any work to them in this, they do represent how you would use GitHub Projects with other people. However, in this solo activity, you'll be assigning issues to yourself! 
---

## Prerequisites

Before starting this lesson, you should be at least a little familiar with:

- Navigation of GitHub (finding repositories, tabs, and getting around the site)
- Creating Repos, Pull Requests, Branches, and the GitHub Workflow

**Estimated Time:** 30–45 minutes

---

## Scenario

You've been put in charge of organizing a school project: your team needs to build a website together. Your job right now isn't to build anything — it's to set up a system so that everyone knows what to do, who is doing it, and when it needs to be done.

You'll be creating issues assigned to each of them and organizing everything using a GitHub Project.

---

## Part 1: Create Your Repository

Your repository is the home base for your project. Everything — your issues, your project board, and eventually your code — lives here.

1. In the upper-right corner of any GitHub page, click your **profile picture**, then click **"Your repositories"**.
1. Click the green **"New"** button in the upper right.
1. Choose your username from the `Owner` dropdown menu (if not already selected).
1. Under **"Repository name"**, type `fake-website-learning-issues-projects`.
1. In the **"Description"** field, type `Practice repo for Project Management`.
1. Under Visibility, select **Public**.
1. No template selected from template dropdown menu.
1. Make sure to toggle the box that says **"Add a README file"** — this gives the repository something to show right away and makes working in your repo possible. Skipping this step will initialize an empty repo and you'll have a bad time.
1. No .gitignore selected from .gitignore dropdown menu.
1. No license selected from dropdown menu.
1. Click **"Create repository"**.

You now have a repository! This is home base for your project.

---

## Part 2: Create a GitHub Project

A **Project** in GitHub is like a digital bulletin board where you can see all your tasks in one place. Think of it like a to-do list that your whole team can see and update.

> 📖 [Learn more about GitHub Projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)

1. From your repository page, click the **"Projects"** tab near the top of the page (next to Code, Issues, etc.).
1. Click the green **"New project"** button.
1. A pop-up will appear with some layout options. Click **"Board"** to select the Kanban-style board layout, which has columns like "Todo", "In Progress", and "Done".
1. In the **"Project name"** field at the top of that same pop-up, type `Website Project Tracker`.
1. Unclick the `Import items from repository` option if it's clicked. 
1. Click **"Create project"**.

Your project board is now created! It will be empty for now — you'll fill it up as you go through this lesson.

---

## Part 3: Create Milestones

**Milestones** are like chapter markers for your project. They let you group a set of tasks under a shared deadline.

> 📖 [Learn more about Milestones](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones)

1. Navigate back to your recently created repository and click the **"Issues"** tab at the top of the page.
2. Near the top right of the Issues page, click the **"Milestones"** button (it's next to a button that says "Labels").
3. Click the green **"New milestone"** button in the upper right.
4. Fill in the details for your first milestone:
   - **Title:** `Week 1 - Planning & Setup`
   - **Due date:** Click the date field and pick a date about one week from today
   - **Description:** `Get the project organized and decide on member roles`
   - Click the green **"Create milestone"** button at the bottom of the form.
5. It should show you your newly created Milestone. Click the `Back to Milestones` link above the title of this Milestone. 
6. Click **"New milestone"** again to create a second one:
   - **Title:** `Week 2 - Building the Site`
   - **Due date:** Pick a date about two weeks from today
   - **Description:** `Complete the main pages and content`
   - Click **"Create milestone"**.

You now have two milestones. When you create issues in the next few steps, you'll attach each one to the right milestone. Stay in the Issues tab for the next steps. 

---
## Part 4: Create and Use Issue Labels

**Labels** are colored tags you can attach to issues to help categorize and filter them. For example, you might label an issue as `design`, `content`, or `urgent` so that at a glance, anyone on the team knows what kind of work it involves.

GitHub gives you a set of default labels automatically (like `bug`, `enhancement`, and `documentation`), but you can also create your own custom labels.

> 📖 [Learn more about Labels](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels)

### Create Custom Labels

1. From your repository page, click the **"Issues"** tab at the top of the page.
2. Near the top right of the Issues page, click the **"Labels"** button (it's right next to the "Milestones" button you used earlier).
3. You'll see a list of labels that GitHub created for you automatically. Take a moment to look them over — you can use these as-is, edit them, or create new ones.
4. Click the green **"New label"** button in the upper right to create your first custom label.
5. Fill in the details for the first label:
   - **Label name:** `design`
   - **Description:** `Visual layout, colors, and appearance tasks`
   - **Color:** Click the small color box on the left to pick a color, or click the refresh icon 🔄 next to the color box to get a random color suggestion. Pick something that feels right for design work. 
> HINT: Picking very different colors for each label makes for easier visual organization later on.  
   - Click **"Create label"**.
6. Click **"New label"** again to create a second label:
   - **Label name:** `content`
   - **Description:** `Writing, editing, and proofreading tasks`
   - **Color:** Pick a different color from the previous label.
   - Click **"Create label"**.
7. Create one more label:
   - **Label name:** `setup`
   - **Description:** `Project structure and configuration tasks`
   - **Color:** One more different color!
   - Click **"Create label"**.

You now have three custom labels ready to use!

---

## Part 5: Create Issues and Assign Them

**Issues** are individual tasks — think of each one like a sticky note. Each issue has a title, a description, an assignee (the person responsible), and a milestone (when it's due).

> 📖 [Learn more about Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)

### Create Issue #1 — Step by Step

Follow these steps carefully for the first issue. You'll use the same process for all the rest.

1. From your repository page, click the **"Issues"** tab at the top.
2. Click the green **"New issue"** button on the right side of the page.
3. In the **"Title"** field near the top, type: `Create homepage wireframe`
4. In the large text box below the title (the description area), type:
   > `Martha will sketch out what the homepage should look like before we start building. This includes deciding on layout, colors, and what sections to include.`
5. Look at the right-hand sidebar on the same page. Find **"Assignees"** and click the gear icon ⚙️ next to it. A small dropdown will appear. (You can click anywhere in line with the gear)
> Since this is a practice exercise with fictional names, you can assign the issue to **yourself** for now. If this were a real project, you would be able to assign anyone inside you had added to the repo as a collaborator. 
6. Click the **Labels** section and add the appropriate label to the issue. This one would be **`design`**.
7. Find **"Milestone"** and click. Select **"Week 1 - Planning & Setup"** from the dropdown.
8. Click the green **"Submit new issue"** button at the bottom of the page.

Your first issue is created! If you click the `Issues` tab above you'll see a list of all your current issues. The issue you just created now appears in your Issues list with a number (like `#1`), the assignee, and the milestone attached. Additionally, labels for the issue show up alongside it in the issue view.

---

### Create the Remaining Issues

Now create the following five issues using the same steps above. For each one:
- Click **"New issue"** from the Issues tab
- Fill in the title and a short description in your own words
- Set the **Assignee** (Again, since this is solo, you'll only be assigning yourself, but you would be able to assign anyone in the repo as a collaborator.)
- Set the **Milestone** based on the table below
- Set the **Label** based on the table below
- Click **"Submit new issue"**

| Issue Title | Fictional Assignee | Milestone | Label |
|---|---|---|---|
| `Write content for the About Us page` | Cindy | Week 1 - Planning & Setup | `content` |
| `Build the navigation bar` | Horton | Week 2 - Building the Site | `setup` |
| `Find and add images to the homepage` | Ted | Week 2 - Building the Site | `design` |
| `Review and proofread all page content` | Cindy | Week 2 - Building the Site | `content` |
| `Set up the project file structure` | Martha | Week 1 - Planning & Setup | `setup` |

When you're done, click back on the **"Issues"** tab and you should see all 6 issues listed with their milestones and labels shown beneath each title.

---

## Part 6: Add Issues to Your Project Board

Now let's connect your issues to your Project so everything is visible in one place.

> 📖 [Adding items to your project](https://docs.github.com/en/issues/planning-and-tracking-with-projects/managing-items-in-your-project/adding-items-to-your-project)

1. Go back to your project board by clicking the **"Projects"** tab in your repository.
1. Click the `Link a project` button to the left of the green `+ New Project` button.
1. Make sure `Website Project Tracker` is checked and click submit. 
1. Click **"Website Project Tracker"** to enter into the project. 
1. You'll see three columns: **Todo**, **In Progress**, and **Done**. Hover over the  **"Todo"** column, and find and click the **"+ Add item"** button.
1. A small text input will appear. Type the `#` symbol into it and select the `fake-website-learning-issues-projects` repo. Click into the search bar to the right and your issues should pop up. 
1. A dropdown list will pop up showing all the issues in your repository. Click on the first issue to add it to the board.
1. Repeat for each remaining issue until all 6 are on the board.

All your tasks are now visible as cards on the board! You can drag and drop cards between columns as work progresses.

>NOTE: You can add issues to projects while creating issues as well. When creating an issue, you can select a project in the same right hand menu where you add milestones and labels. There are multiple ways to do almost everything on GitHub! 
---

## Part 8: Explore Different Project Views

One of the most powerful things about GitHub Projects is that you can view the same information in **different ways** — whatever is most helpful for the situation.

> 📖 [Changing the layout of a view](https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/changing-the-layout-of-a-view)

### Board View
You're already looking at it! Each column represents a stage of work: **Todo**, **In Progress**, and **Done**. This is great for a quick snapshot of what's happening across the whole project.

### Add a Table View
1. At the top-left area of your project, look for a **"+ New view"** button — it appears as a `+` icon next to the tab for your current view. Click it.
2. From the options that appear, select **"Table"**.
3. A new tab will open showing all your issues as rows in a spreadsheet-style layout. You can see each issue's title, assignee, milestone, and status all in one row — great for scanning the full list quickly.

> 💬 **Reflect:** Look at both views you just created. Ask yourself: *"Which view would I want to look at first thing during a work session? Which one would be most helpful for a check-in with the whole team?"* There's no wrong answer — different views are useful for different situations!

---

## Part 9: Update an Issue's Status

Let's simulate some progress on the project by moving issues between columns.

1. Click on the **Board View** tab at the top of your project to go back to the board.
2. Find the card that says `Set up the project file structure`. Click and hold on the card, then drag it from the **"Todo"** column to the **"In Progress"** column. Release it to drop it there.
3. Find the card that says `Create homepage wireframe`. Drag it all the way to the **"Done"** column.

Your board now reflects that some work is underway and some is complete. In a real project, each team member would be responsible for updating their own cards as they make progress.

---

## Best Practices

These aren't required to complete the activity, but they'll make working on GitHub much smoother in the long run:

- **Write clear issue titles** — "Build navigation bar" is much better than "Nav stuff". Anyone on the team should be able to read it and immediately understand the task.
- **Use descriptions generously** — Add as much context as you can in the issue body. Notes, questions, links to references, and sketches are all helpful.
- **Assign one person per issue** — When everyone is assigned to everything, no one feels responsible. One owner per task keeps accountability clear.
- **Everything Gets a Label** - Utilizing these project management tools help teams stay organized, and helps reduce context switching from another application to GitHub. 
- **Check your project board at the start of every work session** — A 2-minute board check-in can replace a 20-minute status meeting.
- **Keep issues updated constantly** - Whenever someone completes work, or even makes some progress on work, they should always add a comment to the issue to indicate what has changed. 
- **Make new Issues for bugs, delays, and important news for the whole team** - Issues and project boards are for communicating between teammates. A well run team knows to check the project board and issues before pinging someone for an update. 
- **Keep milestones realistic** — Don't front-load everything into Week 1. Spread the work out and adjust due dates as the project evolves.
- **Close issues when they're done** — Once a task is truly finished, close the issue. This keeps your board clean and gives the team a sense of progress. Or, if the work is no longer relevant, close it as `Not Planned`. 

---

