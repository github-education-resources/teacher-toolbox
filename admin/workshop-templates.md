# Workshop Templates

We're pleased to offer sample workshop templates you can use in order to lead workshops on using GitHub.


## GitHub First Week Workshop Template

<details><summary>

</summary>

## Workshop Overview

**Audience:** Absolute beginners (students, teachers, or professionals new to GitHub)  
**Duration:** 1 week (can be delivered as a series of daily sessions or a single multi-hour bootcamp)  
**Goal:** By the end of the week, participants should be able to create a GitHub account, understand core version control concepts, collaborate on repositories, and use basic Markdown.

---

## Day 1: Introduction to Git & GitHub

- **Objectives:**
  - Understand what version control is and why it matters.
  - Distinguish between Git and GitHub.
  - Set up a GitHub account.

- **Activities:**
  - Watch: [What is GitHub? (YouTube)](https://www.youtube.com/watch?v=pBy1zgt0XPc)
  - Read: [What is Git? Beginner’s Guide](https://github.blog/developer-skills/programming-languages-and-frameworks/what-is-git-our-beginners-guide-to-version-control/)
  - Hands-on: Sign up for a GitHub account.

---

## Day 2: Creating and Navigating Repositories

- **Objectives:**
  - Create a new repository.
  - Learn about branches, commits, and pull requests.

- **Activities:**
  - Read: [Quickstart for repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories)
  - Watch: [How to create your first repo](https://www.youtube.com/watch?v=-RZ03WHqkaY)
  - Hands-on: Create a repository, add a README.

---

## Day 3: Collaborating with GitHub

- **Objectives:**
  - Understand GitHub Flow (branch, commit, pull request, merge).
  - Learn how to contribute to projects.

- **Activities:**
  - Read: [Introduction to GitHub](https://learn.microsoft.com/en-us/training/modules/introduction-to-github/)
  - Watch: [How to open and merge a pull request](https://www.youtube.com/watch?v=-RZ03WHqkaY)
  - Hands-on: Fork a repository, make a simple change, open a pull request.

---

## Day 4: Issues and Project Management

- **Objectives:**
  - Use GitHub Issues to track tasks.
  - Apply labels, milestones, and assign tasks.

- **Activities:**
  - Watch: [What are GitHub Issues? (YouTube)](https://www.youtube.com/watch?v=6HWw7rhwvtY)
  - Read: [GitHub Issues Quickstart](https://docs.github.com/en/issues/tracking-your-work-with-issues/configuring-issues/quickstart)
  - Hands-on: Create and label issues in your repository.

---

## Day 5: Communicating with Markdown

- **Objectives:**
  - Learn the basics of Markdown for README files, issues, and pull requests.

- **Activities:**
  - Complete: [Communicate Effectively using Markdown (MS Learn)](https://learn.microsoft.com/en-us/training/modules/communicate-using-markdown/)
  - Hands-on: Update your README or an issue with formatted Markdown content.

---

## Day 6: Explore GitHub Copilot (Optional/Advanced)

- **Objectives:**
  - Introduction to GitHub Copilot.
  - Understand how Copilot assists with coding and documentation.

- **Activities:**
  - Read: [Getting Started with Copilot](https://github.com/skills/getting-started-with-github-copilot)
  - Watch: [Getting Started with Copilot Blog & Video](https://github.blog/ai-and-ml/github-copilot/github-for-beginners-how-to-get-started-with-github-copilot/)

---

## Day 7: Showcase and Q&A

- **Objectives:**
  - Review what you’ve learned.
  - Share your first repository with the group.
  - Q&A and troubleshooting.

---

## Additional Resources

- [GitHub Foundations for Non-Developers](https://learn.microsoft.com/en-us/training/modules/introduction-to-github/)
- [Basic Git Commands](https://docs.github.com/en/get-started/using-git/about-git#basic-git-commands)
- [Student Resources & Benefits](https://education.github.com/pack) (if applicable)

---

## Facilitator Tips

- Encourage participants to share their screens and ask questions.
- Use breakout rooms for peer collaboration.
- Provide a shared document or GitHub Discussions board for ongoing support.

---

Happy Coding!

 </details>

 ## Workshop: Creating Your First Python App with GitHub Copilot

 <details><summary>

</summary>

## Overview

**Audience:** Beginners new to Python, GitHub, and Copilot  
**Format:** 1-2 hour hands-on session  
**Objective:** By the end of this workshop, participants will have created a simple Python app from scratch using GitHub Copilot for code suggestions, and committed their work to a GitHub repository.

---

## Agenda

### 1. Introduction (10 min)
- What is GitHub Copilot?
  - [Getting Started with Copilot Blog & Video](https://github.blog/ai-and-ml/github-copilot/github-for-beginners-how-to-get-started-with-github-copilot/)
  - [Intro to GitHub Copilot (Microsoft Learn Module)](https://learn.microsoft.com/en-us/training/modules/introduction-to-github-copilot/)
- What is GitHub? How do we use it for Python projects?

---

### 2. Setup (15 min)
- **Prerequisites:**  
  - GitHub account ([Sign up here](https://github.com/join))
  - Visual Studio Code (VS Code) installed ([Download](https://code.visualstudio.com/))
  - Python installed ([Download](https://www.python.org/downloads/))
- **Enabling Copilot:**
  - [Getting Copilot Set up on Your Account](https://docs.github.com/en/copilot/setting-up-github-copilot/setting-up-github-copilot-for-yourself)
  - Install the GitHub Copilot VS Code extension
- **Create a new repository on GitHub**
  - Title: `first-python-app`
  - Initialize with README

---

### 3. Clone Repository & Set Up Project (10 min)
- Open VS Code
- Clone your new repo (VS Code: `Ctrl+Shift+P` > "Git: Clone")
- Create a new Python file: `app.py`

---

### 4. Guided Coding with Copilot (35 min)
- **Prompt 1:** Write a docstring at the top:  
  _“A simple Python calculator app that adds, subtracts, multiplies, and divides two numbers.”_
- **Prompt 2:** Ask Copilot to generate the function signatures:
  - `def add(a, b):`
  - `def subtract(a, b):`
  - `def multiply(a, b):`
  - `def divide(a, b):`
- **Prompt 3:** Complete each function with Copilot suggestions.
- **Prompt 4:** Ask Copilot for a `main()` function that:
  - Greets the user
  - Asks for two numbers and the operation
  - Calls the appropriate function and prints the result
- **Test your app:**  
  - Run the script in VS Code terminal:  
    ```
    python app.py
    ```
  - Try each operation!

---

### 5. Commit & Push Your Work (10 min)
- Stage and commit your code:  
  - `git add app.py`
  - `git commit -m "Add calculator app"`
  - `git push`
- See your changes on GitHub.

---

### 6. Extension Challenge (Optional, 10+ min)
- Use Copilot to add error handling for invalid input.
- Ask Copilot to add unit tests in a new file named `test_app.py`.

---

## Additional Resources

- [Getting Started with Copilot (GitHub Skills)](https://github.com/skills/getting-started-with-github-copilot)
- [Build a minigame with Copilot and Python](https://learn.microsoft.com/en-us/training/modules/challenge-project-create-mini-game-with-copilot/)
- [Python Docs](https://docs.python.org/3/tutorial/index.html)
- [Communicate Effectively using Markdown](https://learn.microsoft.com/en-us/training/modules/communicate-using-markdown/)

---

## Facilitator Tips

- Encourage participants to experiment with different prompts for Copilot.
- Remind everyone: Copilot is a helper, not a replacement for understanding code!
- Pair up participants to discuss suggestions and learn together.

---

Happy Coding!

 </details>

 ## Workshop: Leveraging GitHub for Professional Development

 <details><summary>

</summary>
---

## Slide 1: Title Slide
- **Title:** Leveraging GitHub for Professional Development
- Presenter’s name and credentials  
- Date

---

## Slide 2: Workshop Objectives & Agenda
- Today’s goals:
  - Understand GitHub’s value for your professional journey
  - Learn how to showcase your work and engage with the community
  - Discover certifications and continuous learning options
- Agenda overview

---

## Slide 3: What is GitHub? Why Professionals Use It
- Brief definition: Git vs. GitHub
- Key features: version control, collaboration, portfolio building
- [Quickstart Guide for Educators](https://docs.github.com/en/education/quickstart)

---

## Slide 4: Professional Benefits of GitHub
- Digital portfolio for your projects
- Open source contributions & networking
- Visibility to recruiters and collaborators
- [GitHub Education for Teachers](https://docs.github.com/en/education/explore-the-benefits-of-teaching-and-learning-with-github-education/github-education-for-teachers)

---

## Slide 5: Creating & Showcasing Your Work
- Demo: Starting a new repository
- Importance of good README and documentation
- Using Issues & Project Boards for project management
- [Quickstart for Repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories)
- [GitHub Issues Guide](https://docs.github.com/en/issues/tracking-your-work-with-issues/configuring-issues/quickstart)

---

## Slide 6: Tips for a Standout Repository
- Clear, descriptive README
- Visuals: badges, screenshots, GitHub Pages
- Organized project structure
- [Basic Writing and Formatting Syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

---

## Slide 7: Engaging with Open Source
- How to find projects: [Good First Issues](https://forgoodfirstissue.github.com/)
- Forking, pull requests, collaboration etiquette
- Benefits: mentorship, skill development, reputation
- [Open Source Guides](https://opensource.guide/)

---

## Slide 8: Managing Your Work with GitHub Issues
- Issues for tracking progress and accountability
- Labels, milestones, and assignees
- [GitHub Issues Learning Path](https://docs.github.com/en/issues/tracking-your-work-with-issues/configuring-issues/quickstart)

---

## Slide 9: Certifications & Continuous Learning
- Overview: GitHub certifications (Foundations, Actions, Advanced Security, Copilot)
- How to prepare: [MS Learn](https://learn.microsoft.com/en-us/training/github/), [Certifications](https://resources.github.com/learn/certifications/)
- [GitHub Skills](https://skills.github.com/) for hands-on learning

---

## Slide 10: Professional Branding on GitHub
- Customizing your profile (profile README, pinned repos)
- Linking GitHub to LinkedIn, resumes, and portfolios
- Example of a strong GitHub profile

---

## Slide 11: Resources & Next Steps
- Curated resource list:
  - [Professional Resources](https://github.com/github-education-resources/teacher-toolbox/blob/main/professional-development/professional-resources.md)
  - [Skills](https://skills.github.com/)
  - [Open Source Learning Path](https://opensauced.pizza/learn/)
- Call to action: Start (or update) your GitHub profile and contribute to a project

---

## Slide 12: Q&A and Discussion
- Open floor for questions
- Invite attendees to share their GitHub profiles or ask for feedback

---

## Slide 13: Thank You!
- Contact information
- Link to slides and resource handout

---

 </details>
