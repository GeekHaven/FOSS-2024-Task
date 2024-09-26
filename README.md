
# Geekhaven FOSS Recruitment Task

Welcome to the Geekhaven FOSS recruitment challenge! We're excited to see how you tackle the tasks and demonstrate your GitHub, SSH, and scripting skills. Read carefully and execute your tasks with precision.

---

## 📚 **Task Overview**

Your goal is to:

- Manage GitHub repositories and permissions.
- Utilize Git hooks to validate commits.
- Work with SSH keys and deploy keys.
- Override commit authorship.
- Test your tasks with Bash scripts.
- As a bonus, integrate GitHub Actions to automate workflow tasks.

---

## 🚀 **Task Steps**

### Step 1: Repository Setup (5 points)

1. **Create a private repository** on GitHub.
2. Add the following GitHub IDs as collaborators:
   - `bhupesh98`
   - `VatsalBhuva11`
3. Perform **a couple of commits** by pushing any of your previous project files to this new repository under the main branch.

### Step 2: Utilize Git hooks (20 points)

1. Create a **pre-commit hook** that logs the last 5 commands you run in a file named `task_commands.sh` in the repository.
2. Make sure this file is **not tracked** by Git.
3. Push this hook to the repository under the folder `hooks` and try it out.
4. Create a **post-commit hook** that logs the commit message and author details in a file named `commit_details.txt` in the repository.
5. Make sure this file is **not tracked** by Git.
6. Push this hook to the repository under the folder `hooks`.
7. At the end of the task,remove these hooks & commit these two files created by hooks inside the `hooks` folder.

### Step 3: Setup SSH Keys and Deploy Keys (10 points)

1. **Logout from GitHub** on the machine you’re working on and the repository locally.
2. Generate **Public** and **Private SSH Keys** using OpenSSH CLI tools. Name these files as `deploy_key.pub` & `deploy_key`.
3. Configure **Deploy Keys** on your repository with the following permissions:
    - Read
    - Write
4. Clone your repository using the SSH URL. It is recommended to configure your SSH config file to use the generated SSH key. Here is an example of how you can do it:

```bash
   Host $YOUR_REPO_NAME
     HostName github.com
     User git
     IdentityFile /path/to/your/private/key
```

### Step 4: Override Commits on a Different Branch (10 points)

1. Create a **new branch** and switch to it.
2. Override some previous commits by **changing the author name** and email (use any desired nickname and alternate email).
3. Push these changes back to your **private repository** under this new branch.

### Step 5: Write a Testing Bash Script (40 points)

Create another **Bash script** that tests whether the tasks perfornmed above are successfully executed. Make sure include **fun and colorful outputs** using **ANSI color codes**:

- Use **blue** for informational messages.
- Use **yellow** for warnings.
- Use **green** for success messages.
- Use **red** for errors.

## Bonus Tasks (Optional)

### 1. Set Up GitHub Actions (15 points)

**Configure a simple GitHub Actions workflow** in your private repository. This workflow should use linting tools like `shellcheck` to check for errors in your scripts & set conditions to only run on desired branch.

### 2. 🎉 Custom Workflow Messages (10 points)

As part of the fun, you can enhance your GitHub Actions workflow by adding **custom, colorful output messages** when running `shellcheck` workflow. This will make your workflow more engaging and help differentiate between errors, warnings, and success messages, just like you did with the Bash script. This will be simple messages based on exit code of the shellcheck commands.

### Step 6: Submit Your Work

Create a **JSON file** containing your details. The JSON file should include:

- Your Name
- Your Roll Number
- Your Email
- The link to your private GitHub repository

Also, push an image to your repository where all the tasks have been verified by your tester bash script.

---

## 📂 **File Naming and Submission Format**

> [!WARNING]
> Please keep your `public key` and `private key` in `.gitignore` file, as you must totally avoid commiting these files in your github repository. But these files must be present locally when executing the test script.

1. Name your files as follows:
   - The script where commands were being logged: `task_commands.sh`
   - The testing script: `task_tester.sh`
   - The information JSON file: `info.json`
   - The GitHub Actions workflow file: `.github/workflows/task_workflow.yml`
   - The image file: `result.png`.
   - Public key: `deploy_key.pub`
   - Private key: `deploy_key`

2. **Create a pull request** on this repository on the main branch where you must make a folder with name as your *Enrollment Number*. Under that, there should be your `info.json` file.

Make sure your submission is neat and follows the required file names and structure. Any deviation might cost you valuable points in this competitive task!

---

## 🎯 **Submission Guidelines**

- **Do NOT share** or expose your SSH keys or other sensitive data publicly.
- Your private repository should have **proper collaborator permissions** for the IDs mentioned above.
- Make sure your Bash script runs seamlessly on any standard Linux/Unix environment.
- Pay attention to detail and ensure everything is automated as per the requirements.
- Do not use AI tools for completion of this task. We are looking for your skills and not the AI's. We know most of you might not have heard some of these tooling before, but that's the point of this task. To learn and implement new things. Learn concepts (here your AI might help you) and implement them on your own.

---

We’re looking forward to seeing your submissions! Best of luck and have fun with this challenge. 👾
Shall you have any doubts, feel free to contact either of the organizers to resolve them. Irrelevant doubts will not be entertained/will be ignored. You should try resolving them on your own first, and only if the solution is not immediately obvious or found to you, only then contact us. ([@bhupesh98](https://github.com/bhupesh98/) , [@VatsalBhuva11](https://github.com/VatsalBhuva11)).
