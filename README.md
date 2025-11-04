# Projects Repo

> This repository holds the Markdown sources that  **[Project Viewer](https://github.com/rileybarshak/project-viewer)** displays in a clean, sortable gallery.  
> This repo is focused on your projects, the viewer handles all rendering and presentation.

---

## Basic Structure

```text
projects/
  Completed/
    Finished Project Name/
      finsihedproject.md
  In Progress/
    Building Right Now/
      buildingnow.md
  Incomplete/
    Not Started/
      notstarted.md
  Uncategorized Example/
    nostatus.md
```

- The viewer automatically detects **Completed**, **In Progress**, and **Incomplete** as project status categories.  
- Any other top-level folder is treated as **Uncategorized**.

---

## Markdown File Format

Each project folder should contain at least one `.md` file following this template:

```markdown
# My Project
> **Project Type:** Personal project
> **Project Description:** Quick description that appears on the card.
> **Project Goal:** Goal of the project
> **Languages & Technologies:** TypeScript, React, Next.js, Tailwind CSS
```

If you'd like the card to redirect to another page instead of opening the markdown file, change line 1 to `[My Project](https://example.com/demo)`

The viewer uses:
- Line 1: project name for the project card.
- Line 3: (`**Project Description:** …`) for the card blurb.
- Line 5: (`**Languages & Technologies:** …`) for tags (comma-separated, case-insensitive).

---

## Setting Up the Viewer

**Repository:** [rileybarshak/project-viewer](https://github.com/rileybarshak/project-viewer)

- A **Next.js** web app that reads this `projects` repository and displays each Markdown file as a project card and detail page.  
- Configure your viewer by setting `GITHUB_USER=<your-github-username>` in the viewer’s `.env` file.  
- Deploy the viewer (for example, on **Vercel**) and it will automatically load and display your projects from this repo.

---

## Tips

- Place images in the same project folder as where they are being used so they render correctly in the viewer:
  ```markdown
  ![Screenshot](screenshot.png)
  ```
- Keep folder names simple and readable.  
- Push commits: your viewer will update automatically within a minute.

---

## That’s It!

Add folders and Markdown files following this structure, the Project Viewer will handle everything else automatically.
