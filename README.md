
# Geekhaven FOSS Recruitment Task

Welcome to the Geekhaven FOSS recruitment challenge! We're excited to see how you tackle the tasks and demonstrate your GitHub, SSH, and scripting skills. Read carefully and execute your tasks with precision.

---

## 📚 **Task Overview**

Your goal is to:
- Manage GitHub repositories and permissions.
- Work with SSH keys and deploy keys.
- Override commit authorship.
- Automate your tasks with Bash scripts.
- Use ANSI color codes to style your output.
- As a bonus, integrate GitHub Actions to automate workflow tasks.

---

## 🚀 **Task Steps**

### Step 1: Repository Setup (5 points)
1. **Create a private repository** on GitHub.
2. Add the following GitHub IDs as collaborators:
   - `bhupesh98`
   - `VatsalBhuva11`
3. Perform **a couple of commits** by pushing any of your previous project files to this new repository.

### Step 2: Setup SSH Keys and Deploy Keys (10 points)
1. **Logout from GitHub** on the machine you’re working on.
2. Generate **Public** and **Private SSH Keys** using OpenSSH CLI tools.
3. Configure **Deploy Keys** on your repository with the following permissions:
    - Read
    - Write

### Step 3: Override Commits on a Different Branch (10 points)
1. Create a **new branch** and switch to it.
2. Override some previous commits by **changing the author name** and email (use any desired nickname and alternate email).
3. Push these changes back to your **private repository** under this new branch.

### Step 4: Automate Everything with a Bash Script (50 points)
Write a Bash script that automates the following:
- Logging out from GitHub.
- Generating SSH keys.
- Setting up deploy keys.
- Creating a new branch.
- Overriding commits with a custom author name and email.
- Pushing these changes back to your private repository.

Ensure the script is clearly documented with comments.

### Step 5: Write a Testing Bash Script (40 points)
Create another **Bash script** that tests whether the tasks in Step 4 are successfully executed. Make sure to:
- Include **fun and colorful outputs** using **ANSI color codes**:
  - Use **blue** for informational messages.
  - Use **yellow** for warnings.
  - Use **green** for success messages.
  - Use **red** for errors.

## Bonus Tasks (Optional)
### 1. Set Up GitHub Actions (15 points)
**Configure a simple GitHub Actions workflow** in your private repository. This workflow should:
1. Ensure that the script executes successfully without errors. If there are any issues, the workflow should fail and notify you.
2. Extend the workflow to include linting tools like `shellcheck` to check for errors in your scripts or set conditions to only run on specific branches.

### 2. 🎉 Custom Workflow Messages (5 points)
As part of the fun, you can enhance your GitHub Actions workflow by adding **custom, colorful output messages**. This will make your workflow more engaging and help differentiate between errors, warnings, and success messages, just like you did with the Bash script.

### Step 6: Submit Your Work
Create a **JSON file** containing your details. The JSON file should include:
- Your Name
- Your Roll Number
- Your Email
- The link to your private GitHub repository

---

## 📂 **File Naming and Submission Format**

1. Name your scripts as follows:
   - The automation script: `task_automation.sh`
   - The testing script: `task_tester.sh`
   - The information JSON file: `info.json`
   - The GitHub Actions workflow file: `.github/workflows/task_workflow.yml`

2. **Create a pull request** on the public repository (where these tasks are made live) with the following:
   - **Branch Name:** `your-rollnumber_submission`
   - Your pull request must contain:
     - `task_automation.sh`
     - `task_tester.sh`
     - `info.json`
     - `.github/workflows/task_workflow.yml`

Make sure your submission is neat and follows the required file names and structure. Any deviation might cost you valuable points in this competitive task!

---

## 🎯 **Submission Guidelines**

- **Do NOT share** or expose your SSH keys or other sensitive data publicly.
- Your private repository should have **proper collaborator permissions** for the IDs mentioned above.
- Make sure your Bash script runs seamlessly on any standard Linux/Unix environment.
- Pay attention to detail and ensure everything is automated as per the requirements.

---

We’re looking forward to seeing your submissions! Best of luck and have fun with this challenge. 👾
Shall you have any doubts, contact either of the organizers to resolve them. Irrelevant doubts will not be entertained/will be ignored. You should try resolving them on your own first, and only if the solution is not immediately obvious or found to you, only then contact us. (@bhupesh98 , @VatsalBhuva11)
