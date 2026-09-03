# SRT111-Lab0 - Environment Setup and GitHub Repository Configuration
This lab will help you setup the enviroment needed to complete the labs on your personal laptop.
It is recommended that you bring your own laptop to each class.
This lab must be completed before the first class of week 2.

## Objectives:
By the end of this lab, you will:

- Install Python, VS Code, and Git on your personal laptop.
- Configure Git with your Seneca information.
- Create your course GitHub repository.
- Add your professor as a collaborator.
- Clone your repository to your computer.
- Create and run your first Python program.
- Commit and push your work to GitHub.

## Introduction
Throughout this course, you will maintain one GitHub repository named:
``` YAML
SRT111F2026
```
This repository will contain all of your lab work for the semester.
As new labs are assigned, you will create folders inside this repository and store your work there.
``` text
SRT111F2026
├── Lab00
├── Lab01
├── Lab02
├── Lab03
└── ...
```
For each lab, you will:
- Download the starter files provided by your professor.
- Create a new lab folder in your local copy of the repository.
- Complete the lab activities using VS Code.
- Commit your changes using Git.
- Push your work to GitHub.
 
By completing this lab, you will set up all the software and accounts required for the remainder of the course.

**Important:** You will create **one repository for the entire semester**. Each lab will be stored in its own folder within that repository. The repository will exist both on GitHub.com and on your computer. Git is used to keep these two copies synchronized.
  
---

## Part 1: Install Required Software

Before you can begin working on course labs, you must install the software used throughout the semester.
We will use the following tools:
- **Anaconda** - Anaconda provides everything needed for this course in a single installation. Rather than installing Python, Jupyter, and other tools separately, Anaconda bundles them together and makes them easier to manage.
- **Git** - Used to save versions of your work and upload your files to GitHub
  
You only need to complete this setup once.

### Step 1: Install Anaconda

Anaconda includes:
- Python
- Jupyter Lab
- VS Code
- Package management tools
- Common data science libraries
- Many other tools... 

Visit: https://www.anaconda.com/download

Download and install the version appropriate for your operating system. Use the default installation settings unless instructed otherwise.

**Verify the Installation**: After installation, launch **Anaconda Navigator**. Anaconda Navigator is a graphical application that allows you to launch the tools included with Anaconda without using the command line.

You should see applications such as:

- Anaconda Prompt
- Jupyter Notebook
- JupyterLab
- Visual Studio Code

If Anaconda Navigator opens successfully, your installation is complete.
If VS Code does not appear in Anaconda Navigator, install VS Code separately from https://code.visualstudio.com/


### Step 2: Launch VS Code

VS Code is the editor we will use throughout the semester for labs. Open Anaconda Navigator and click Launch under VS Code.

### Step 3: Install the Python Extension
Although Anaconda installs Python and VS Code, the VS Code does not automatically include all of the tools needed to work effectively with Python. The Python extension adds Python-specific features to VS Code, such as:
- Running Python programs directly from VS Code
- Code completion
- Syntax highlighting
- Debugging

Without the Python extension, VS Code behaves like a general text editor. You would still be able to write Python code, but many of the features that make programming easier would be unavailable.
To install the extension:
- Open VS Code
- Select the Extensions icon from the left sidebar
- Search for: `Python`
- Install the extension published by Microsoft
- If prompted, restart VS Code

### Step 4: Verify Installation
After installation, create a new Python file named:
```text
test.py
```
This file is only used to verify your installation and does not need to be submitted. Add the following code:
```Python
print("Hello, SRT111!")
```
You should see Python-related features such as:

- Syntax highlighting
- Python language support in the bottom status bar
- A "Run Python File" option near the top-right corner of the editor

Run the program using the Run Python File button in VS Code.
Expected output:
```text
Hello, SRT111!
```
If the program runs successfully, then Python and VS Code are installed successfully.

### Step 5: Install Git
Git is a version control system that allows you to:

- Save versions of your work
- Track changes to your files
- Upload your work to GitHub
- Maintain your course repository throughout the semester

Throughout this course, you will use Git to save and upload your lab work.

**Download Git:**
- Visit: https://git-scm.com/downloads
- Download and install Git for your operating system.
- Use the default installation settings.

**Verify the Git Installation:**
Inside VS Code, Open a terminal like powershell and run:
```text
git --version
```
Example output:
```text
git version 2.51.0
```
Your version number may be different.
If Git displays a version number, the installation was successful.


## Part 2: Access Your Seneca GitHub Account
Open your web browser and visit: https://github.com/Seneca-Polytechnic

Sign in using your Seneca credentials or SSO.

Your Seneca GitHub account is different from a personal GitHub account that you may have created yourself. 
Be sure to sign in using your Seneca-managed GitHub account. If you are already signed into a personal GitHub account, sign out before signing in with your Seneca account.
After signing in, click your profile picture in the top-right corner of GitHub. Your GitHub username should be displayed which will look like this:
```text
john-smith_seneca
```

## Part 3: Configure Git
Git records who makes changes to files. Before using Git, you must configure your name and email address.

Open a terminal in VS Code and run the following commands:
```Python
git config --global user.name "Your GitHub Username"
git config --global user.email "your.seneca@email.com"
```

Example:

```Python
git config --global user.name "john.smith_seneca"
git config --global user.email "john.smith@myseneca.ca"
```

## Part 4: Create Your Course Repository
Throughout the semester, you will store all lab work in a single GitHub repository.
While signed in to your Seneca GitHub account:

- Click the + button in the upper-right corner.
- Select New Repository.
- Enter the repository name:
```text
SRT111F2026
```
- Set the repository visibility to **Private**.
- Check: Add a README file
- Click Create Repository
- Your repository URL will look similar to: https://github.com/your-seneca-username/SRT111F2026

## Part 5: Add Your Professor as a Collaborator
Your professor will require access to your repository to distribute starter files and review your work.
Inside your repository:

- Click Settings
- Select Collaborators and Teams from the left menu.
- Click Add People
- Search for your professor's GitHub username
- Select the account and send the invitation.
  
## Part 6: Clone the Repository to Your Computer
Now that the repository exists on GitHub, create a local copy on your computer.
- From your GitHub repository page, click the green drop down: `Code`
- Copy the HTTPS URL which may look like this: https://github.com/your-seneca-username/SRT111F2026.git
- Inside VS Code: open a terminal
- Navigate to the location where you want to store your course work.
- Example
``` text
cd /users/john/SRT111/
```
- run the command:
```Python
git clone https://github.com/your-seneca-username/SRT111F2026.git
```
- Move into the repository folder:
```
cd SRT111F2026
```

## Part 7: Create Your Lab00 Folder
Inside your local repository that you just cloned, create a new folder:
```
Lab00
```
Your folder structure should look like:
```text
SRT111F2026
├── README.md
└── Lab00
```

## Part 8: Create Your First Python Program
- Inside the Lab00 folder, create a file named:
```Python
hello.py
```
- Add the following code:
```Python
print("Hello, SRT111!")
print("My GitHub setup is working.")
```
- Run the program inside VS Code to make sure that you get the expected output.

## Part 9: Commit Your Work
Git requires changes to be committed before they can be uploaded.
- Run the following command to **view modified files**:
```
git status
```
- You should see the following listed as untracked file. This is becasue yoru local repository contains this folder and file but this is not yet available in the GitHub.com.
```
Lab00/hello.py
```
- **Stage the files**
```
git add .
```
- Create a commit
```
git commit -m "Complete Lab00 setup"
```
- Upload your changes to GitHub.
```
git push
```
- After the push completes successfully, refresh your GitHub repository page.You should see:
``` text
README.md
Lab00/
    hello.py
```

# Submission Requirements
To receive credit for Lab00, verify that:
- Anaconda is installed
- VS Code launches successfully
- Git is installed
- Git is configured with your Seneca email
- Repository named SRT111F2026 exists
- Professor has been added as a collaborator
- Repository has been cloned to your computer
- Lab00 folder exists
- hello.py runs successfully
- Changes have been committed
- Changes have been pushed to GitHub
