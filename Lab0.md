# SRT111-Lab0 - Environment Setup and GitHub Repository Configuration

## Objectives:
By the end of this lab, you will:

- Install Python, VS Code, and Git.
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

**Important** You will create **one repository for the entire semester**. Each lab will be stored in its own folder within that repository.
  
---

## Part 1: Install Required Software

Before you can begin working on course labs, you must install the software used throughout the semester.
We will use the following tools:
- **Anaconda** - Anaconda provides everything needed for this course in a single installation. Rather than installing Python, Jupyter, and other tools separately, Anaconda bundles them together and makes them easier to manage.
- **Git** - Used to save versions of your work and upload your files to GitHub
  
You only need to complete this setup once.

### Step 1: Install Anaconda

Anaconda includes
- Python
- JupyterLab
- VS Code
- Package management tools
- Common data science libraries
- Many other tools... (you don't need them in this course though)

Visit: https://www.anaconda.com/download

Download and install the version appropriate for your operating system. Use the default installation settings unless instructed otherwise.

**Verify the Installation**: After installation, launch **Anaconda Navigator**. Anaconda Navigator is a graphical application that allows you to launch the tools included with Anaconda without using the command line.

You should see applications such as:

- JupyterLab
- Visual Studio Code

If Anaconda Navigator opens successfully, your installation is complete.


### Step 2: Launch Visual Studio Code

Visual Studio Code (VS Code) is the editor we will use throughout the semester.
Open Anaconda Navigator and click Launch under Visual Studio Code.

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

### Step 3: Verify Installation
After installation, create a new Python file named:
```text
test.py
```
Add the following code:
```Python
print("Hello, SRT111!")
```
You should see Python-related features such as:

- Syntax highlighting
- Python language support in the bottom status bar
- A "Run Python File" option near the top-right corner of the editor

If these features are available, the Python extension has been installed successfully.
