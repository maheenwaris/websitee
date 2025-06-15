---
title: "Creating a GitHub Account, Publishing a Repository, and Pushing Code"
author: "Maheen Waris"
description: ""
url: "/blogs/GitHub-Account/"
date: "2023-09-17"
tags: ["Github", "Guide"]
draft: "false"
toc: "true"
---

GitHub is a popular platform where people can store and share their code. It's a great place for beginners to learn about coding and collaborate on projects with others. In this guide, we will walk you through the steps of creating a GitHub account, publishing a repository (a place to store your code), and pushing your code to the repository. Let's get started!

## Creating a GitHub Account:

### 1. Go to GitHub:

Open your web browser and go to the GitHub website: [www.github.com](https://www.github.com).

### 2. Sign Up:

Click on the "Sign Up" button. You will need to provide some information like your username, email address, and a password. Choose a username that represents you or your projects.

### 3. Choose a Plan:

GitHub offers free plans for individuals. You can choose the free plan by clicking on the "Choose Free" button.

### 4.Verify Your Email:

After signing up, GitHub will send a verification link to the email address you provided. Click on the link to verify your email.

<hr>

## Publishing a Repository

### 1. Login:

Once your email is verified, go back to the GitHub website and log in with your new account.

### 2.Create a New Repository:

Click on the "+" sign in the upper right corner of the GitHub page and select "New Repository."

## 3. Repository Settings:

Repository Name: Choose a name for your repository. This is how it will be identified.
Description: Add a short description to help others understand what your repository is about.
Public or Private: You can choose to make your repository public (visible to everyone) or private (only visible to you and collaborators).

## 4. Create Repository:

Click the "Create repository" button. Your new repository is now set up and ready to hold your code!

<hr>

## Pushing Code to Your Repository

### 1. Clone Repository:

To add your code to the repository, you first need to copy it to your computer. This is called "cloning" the repository. On the repository page, click the green "Code" button and then click the clipboard icon to copy the repository's web address.

### 2. Open Terminal (Command Prompt):

On your computer, open the terminal (on macOS) or command prompt (on Windows).

### 3. Navigate to a Folder:

Use the "cd" command to navigate to the folder where you want to store your code locally.

### 4. Clone the Repository:

In the terminal or command prompt, type `git clone` followed by the web address you copied. Press Enter. This will download the repository to your computer.

```html
git clone https://github.com/your-username/your-repository.git
```

### 5. Add Your Code:

Now, copy your code into the cloned repository folder.

### 6. Push Your Code:

- In the terminal or command prompt, navigate to the repository folder using the `cd` command.
- Type the following commands to add and commit your code:

```html
git add . git commit -m "Add my first code"
```

- Finally, push your code to GitHub with the following command:

```html
git push origin main
```

Congratulations! Your code is now on GitHub.

<hr>

Remember, this guide covers the basic steps to get you started with GitHub. There's a lot more you can explore, like collaborating with others, creating branches, and managing issues. GitHub has a helpful guides section (https://guides.github.com/) that can provide more in-depth information as you continue your coding journey. Happy coding!

<script src="https://utteranc.es/client.js"
        repo="maheenwaris/Website"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>

---
