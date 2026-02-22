# Project Viewer
> **Project Type:** Personal project   
> **Project Description:** Configurable & customizable projects showcase   
> **Project Goal:** Create a visually appealing, efficient, and intuitive project page that is easy to set up and configure.  
> **Languages & Technologies:** TypeScript, React, Next.js, Tailwind CSS   



<h1 style="color:red; margin-bottom: 0;">DEPRECATED</h1>
<h4 style="margin-top: 0;">
  This project will no longer receive updates. See
  <a href="/Incomplete/">Project Viewer V2</a>
</h4>



## [Project Viewer](https://github.com/rileybarshak/project-viewer)

A collection of my projects in various stages of completion. Click on any project to explore its documentation and resources. Designed to be easily configurable and customizable when forked. 
- Used on my [projects page](https://projects.rileyb.net)
- Dynamically pulls content from the [projects repo](https://github.com/rileybarshak/projects) on github
	- Gets name from directory
	- Gets description from line 3 of markdown
	- Gets tags from line 5 of markdown
		- Colors tags based on category (Languages, Frameworks, Libraries, etc)
	- Gets completion status from parent directory
		- Colors folder icon based on completion status (Completed: green, In progress: orange, Incomplete: red)
- Sort by completion status (then alphabetically)
- Click on project to open renderd markdown file from project directory
	- if project name (line 1) is a link, redirect to it instead 


### Core features

 - Automatically builds project cards from folders in the GitHub projects repo
   - Reads metadata from Markdown (template-based):
     - project name (line 1)
     - description (line 3)
     - tags/technologies (line 5)
   - Infers project status from parent folder:
     - Completed
     - In Progress
     - Incomplete
     - otherwise Uncategorized
   - Color-code status badges/folder icons and tag badges
 - Supports search + filters (name, status, tags)
 - Renders project docs by opening and displaying Markdown files from the selected project folder
 - Optional redirect behavior: if the Markdown title is a link, the project card opens that URL instead of the internal page

### How it works 

 - Uses the GitHub Contents API to fetch project folders/files
 - Parses Markdown to extract card metadata (description/tags)
 - Builds a project gallery on the homepage
 - Clicking a project opens a detail page that renders its Markdown with react-markdown
 - Relative links/images in Markdown are rewritten to GitHub/raw GitHub URLs so assets load correctly
 - Most customization is handled in config.yaml:

   - GitHub username
   - tag categories/colors
   - status color styles



