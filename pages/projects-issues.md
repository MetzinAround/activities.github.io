---
layout: default
title: Project Management with GitHub
nav_order: 4
permalink: /project-management/
---

# 45-Minute Workshop: GitHub Issues + Projects (Kanban) — “Plan a Party” (Whole Class, One Repo)

This workshop is designed for **beginners** and focuses on learning the **GitHub UI workflow**, not coding. Everyone in the class will work inside **one repository** created by the Host, using **Issues** and **GitHub Projects** to plan a party.

You will practice:
- Creating **issues** (tasks)
- Adding **labels** (organization)
- Assigning issues to yourself (**assignees**)
- Using **comments** and **@mentions** (conversation + collaboration)
- Adding issues to a **Project board** (kanban)
- Moving issues through **statuses** (Todo → In Progress → Done)
- Using a **milestone** to track progress toward “Party Day”

> **Accounts:** Works with **GitHub Free or Pro** accounts. **No GitHub Enterprise and no GitHub Organizations** required.

---

## Prerequisites (What learners should have)

- A **GitHub Free or Pro** account
- A web browser (Chrome/Firefox recommended)
- Ability to open links and switch between browser tabs
- Basic typing and copy/paste skills
- Your GitHub username (you can find it by clicking your profile picture → **Your profile**)

---

## Helpful GitHub Documentation (Official)

- About Issues: https://docs.github.com/en/issues/tracking-your-work-with-issues/learning-about-issues/about-issues  
- Issue Quickstart (labels, assignees, milestones, projects): https://docs.github.com/en/issues/tracking-your-work-with-issues/learning-about-issues/quickstart  
- About Projects: https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects  
- Changing the layout of a Project view (Table/Board): https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/changing-the-layout-of-a-view  
- Managing labels: https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels  
- About milestones: https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones  

---

## Roles (Virtual-Friendly)

- **Host (Instructor/TA):** Creates the repo, invites learners, sets up labels, milestone, and Project board.
- **Learners:** Each person creates one issue, adds labels, assigns it, comments, @mentions, adds to the Project, and moves status.

---

## Timing Overview (45 minutes)

1. **0–5 minutes:** Host creates repo + invites learners  
2. **5–10 minutes:** Host creates milestone + labels  
3. **10–15 minutes:** Host creates Project board (kanban)  
4. **15–25 minutes:** Learners create and configure one issue each  
5. **25–33 minutes:** Learners add issues to the Project + move across statuses  
6. **33–40 minutes:** Learners practice comments + @mentions  
7. **40–45 minutes:** Milestone progress + label filtering + quick brainstorm

---

# Instructions (Step-by-Step)

## Part 1 — Host: Create the shared repository (0–5 minutes)

1. Go to https://github.com and sign in.
2. In the top-right corner, click your **profile picture**.
3. Click **Your repositories**.
4. Click the green **New** button.
5. Fill out the form:
   - **Repository name:** `party-planning-class` (or a name you choose)
   - **Description:** `Class practice repo for GitHub Issues + Projects`
   - Choose **Public** (recommended) or **Private** (either is fine)
   - Check **Add a README file**
6. Click **Create repository**.

### Host: Invite learners as collaborators (still within minutes 0–5)
1. In the repository, click **Settings** (near the top of the repo).
2. In the left sidebar, click **Collaborators** (sometimes called **Collaborators and teams**).
3. Click **Add people**.
4. In the search box, type a learner’s GitHub username, click the correct account, then click **Add**.
5. Repeat for all learners.

### Learners: Accept the invitation (during minutes 0–5)
1. On GitHub, click the **bell icon** (notifications) near the top-right of the page.
2. Find the repository invitation.
3. Click **Accept invitation**.

> **Virtual tip:** If you’re on a video call, keep the meeting open in one window and GitHub in another window or browser tab.

---

## Part 2 — Host: Create ONE milestone and FOUR labels (5–10 minutes)

### Create the milestone: “Party Day”
1. In the repository, click **Issues**.
2. Near the top of the Issues page, click **Milestones**.
3. Click **New milestone**.
4. Fill in:
   - **Title:** `Party Day`
   - **Due date:** pick a date 1–2 weeks from today (example: `2026-04-03`)
   - (Optional) Description: `Everything needed before the party.`
5. Click **Create milestone**.

### Create four labels (minimal set)
1. In the repository, click **Issues**.
2. Click **Labels**.
3. Click **New label** and create these labels one at a time:

- `food-drinks` — snacks, drinks, ice, cups
- `decor-setup` — decorations, seating, cleanup supplies
- `music-activities` — playlist, games, speakers
- `needs-decision` — blocked until someone chooses/approves

> Keep labels to **4** for this workshop to reduce confusion and help learners focus on the UI.

---

## Part 3 — Host: Create the Project board (kanban) (10–15 minutes)

1. In the repository, click **Projects**.
   - If you do not see **Projects**, click **…** (More) and look for it.
2. Click **New project**.
3. Name the project: `Party Planning Board (Class)`.
4. Create the project.
5. Ensure the layout is a kanban board:
   - Look for the view layout controls near the top of the project.
   - Choose **Board** layout (kanban).

### Check the board columns (statuses)
You should have at least three columns similar to:
- **Todo**
- **In Progress**
- **Done**

If your board shows different names, that is okay as long as learners can move items across statuses.

---

## Part 4 — Learners: Create ONE issue each (15–25 minutes)

Each learner will create **one** party-planning task as a GitHub Issue.

### Step-by-step: Create your issue
1. Open the shared repository link from the Host.
2. Click **Issues** (top of the repo).
3. Click **New issue**.
4. In the **Title** field, type a title using this format:

   `Party Task: <your task>`

   Example: `Party Task: Suggest two drink options`

5. In the large description box, copy/paste this template, then fill it in:

   - **What I’m doing:**  
   - **What “done” looks like:**  
   - **Steps:**  
     - [ ] Step 1  
     - [ ] Step 2  
   - **Question for the team:**  

6. On the **right side** of the issue page, set:
   - **Assignees:** Click **Assignees**, then click **your own username**
   - **Labels:** Click **Labels**, then pick **one** label (only one)
   - **Milestone:** Click **Milestone**, then choose `Party Day`
7. Click **Submit new issue**.

### Suggested issue ideas (choose one)
- `Party Task: Pick a theme/colors` (label: `decor-setup`)
- `Party Task: Suggest 3 snack ideas` (label: `food-drinks`)
- `Party Task: Create a 10-song playlist starter` (label: `music-activities`)
- `Party Task: Decide start time (6pm vs 7pm)` (label: `needs-decision`)

---

## Part 5 — Learners: Add your issue to the Project + move status (25–33 minutes)

You can add issues to the Project in two ways. Try **Option A** first.

### Option A: Add to Project from inside your Issue
1. Open your issue.
2. On the right side of the issue, find **Projects**.
3. Click **Projects**.
4. Select `Party Planning Board (Class)`.

### Option B: Add to Project from inside the Project board
1. In the repository, click **Projects**.
2. Open `Party Planning Board (Class)`.
3. Find **Add item** (a button or a row where you can type).
4. Type the title of your issue and select it when it appears.

### Move your issue across statuses (practice)
1. On the Project board, find your issue card.
2. Drag it from **Todo** to **In Progress**.
3. Wait a moment so others can do the same.
4. Drag it from **In Progress** to **Done**.

> For this workshop, “Done” means “I practiced moving the card,” not “the real-world task is completed.”

---

## Part 6 — Learners: Practice conversation with comments + @mentions (33–40 minutes)

### A. Comment an update
1. Open your issue.
2. Scroll down to the comment box.
3. Type a short update, for example:

   `Update: Here are my ideas. Which option should we choose?`

4. Click **Comment**.

### B. @mention a classmate (or the Host) and ask a question
1. In the same issue, add a second comment.
2. Type `@` and begin typing a username.
3. Click the username from the dropdown list.
4. Ask a question, for example:

   `@username Which of these should we pick? Option A or Option B?`

5. Click **Comment**.

> **Virtual tip:** If you don’t know another learner’s username, @mention the Host so you can still practice the workflow.

---

## Part 7 — Whole class: Review milestone progress + filter by label (40–45 minutes)

### View the milestone progress bar
1. In the repository, click **Issues**.
2. Click **Milestones**.
3. Click `Party Day`.
4. Notice the progress bar showing how many issues are open vs closed.

### Filter Issues by label
1. Go back to **Issues**.
2. Find the label filter (or click **Labels** and choose one).
3. Select `food-drinks` (or another label).
4. Observe how the list changes to show only issues with that label.

### Quick reflection (1–2 minutes)
As a group, answer:
- Where could you use this same workflow in real life (non-coding)?
  - Examples: event planning, class projects, job search checklist, moving plan, volunteer coordination, content calendar.

---

## Best Practices (Helpful tips, not required)

- **Keep labels small and meaningful.** Start with 4–6 labels; expand later if needed.
- **Use action-based issue titles** (start with a verb): “Choose…”, “Decide…”, “Create…”, “Buy…”.
- **Assign issues to yourself** so ownership is clear; use comments for collaboration.
- **Use milestones as deadlines** (Party Day, Launch Day, Move Day, Exam Week).
- **Use Projects as your “status dashboard.”** Use Issues for details, notes, and decisions.
- For quick edits in a repository (like updating a README), you can press the **period key (`.`)** while viewing the repo to open GitHub’s web editor.

---

## Troubleshooting (Common issues in virtual workshops)

- **I can’t assign issues to myself:** You may not have accepted the collaborator invite yet. Click the bell icon and accept the invitation.
- **I can’t find Projects:** Make sure you are in the correct repository, and look for **Projects** in the top navigation (or under **… More**).
- **My issue isn’t on the board:** Adding an issue to a repo does not always automatically add it to the Project. Use the **Projects** picker on the Issue or **Add item** in the Project.