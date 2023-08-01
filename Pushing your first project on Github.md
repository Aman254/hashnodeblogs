---
title: "Pushing your first project on Github:"
seoTitle: "Pushing Your Project on GitHub: A Step-by-Step Guide for Developers"
seoDescription: "Learn how to push your project on GitHub with this comprehensive step-by-step guide. From setting up your GitHub account to connecting your local repository"
datePublished: Mon Jul 10 2023 17:59:09 GMT+0000 (Coordinated Universal Time)
cuid: cljx63t6c000409lgcrcxeymf
slug: pushing-your-first-project-on-github
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689011679084/f9304cba-21bb-4463-b34a-561a3af8b744.jpeg
tags: webdevelopment, github, version-control, terminal-command, wemakedevs

---

Make sure you have your GitHub account created and Dowloaded Git Bash to execute these commands:

Download Git Bash Here: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Introduction: GitHub has revolutionized the way developers collaborate and share their projects with the world. Whether you're working on a personal project or contributing to an open-source repository, pushing your project to GitHub is an essential step. In this blog post, we will guide you through the process of pushing your project onto GitHub, enabling you to showcase your work and collaborate with others.

**Step 1:** Set Up Your GitHub Account and Create a Repository If you haven't already, start by creating a GitHub account. Once you're logged in, click on the "+" button on the top-right corner of the GitHub homepage and select "New repository." Provide a name for your repository, add an optional description, and choose whether it should be public or private.

**Step 2:** Initialize Git in Your Project Directory To track changes and push your project to GitHub, you need to initialize Git in your project directory. Open your terminal or command prompt, navigate to the root directory of your project, and run the following command:

```sql
git init
```

This command initializes a new Git repository in your project directory.

**Step 3:** Add and Commit Your Project Files Now, you need to add the files in your project directory to the Git repository. Run the following command:

```sql
git add .
```

This command adds all the files in your project directory to the staging area. If you want to add specific files, replace `.` with the file names.

Next, commit your changes with a descriptive message using the following command:

```sql
git commit -m "Initial commit"
```

Replace "Initial commit" with an appropriate message summarizing the changes you made in this commit.

**Step 4:** Connect Your Local Repository to GitHub To push your project to GitHub, you need to establish a connection between your local repository and the remote repository on GitHub. On your GitHub repository's page, copy the repository URL.

In your terminal or command prompt, run the following command to add the remote repository:

```sql
git remote add origin <repository_url>
```

Replace `<repository_url>` with the URL you copied.

**Step 5:** Push Your Project to GitHub Now, it's time to push your project to GitHub. Run the following command:

```perl
git push -u origin master
```

This command pushes your project's code to the remote repository on GitHub. The `-u` flag sets the upstream branch, allowing you to simply use `git push` for future pushes.

**Step 6:** Verify Your Project on GitHub Once the push is complete, navigate to your GitHub repository's page and refresh it. You should now see your project files and commits displayed.

***Congratulations!*** You have successfully pushed your project to GitHub. From here on, you can continue to make changes, create branches, and collaborate with others by pushing and pulling code to and from GitHub.

Conclusion: Pushing your project to GitHub is a crucial step in sharing your work and collaborating with other developers. By following the step-by-step guide provided in this blog post, you should now have the knowledge and confidence to push your projects onto GitHub. Embrace the power of version control and explore the numerous opportunities GitHub offers for collaboration and community engagement. Happy coding!
