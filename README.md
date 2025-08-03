# Web Scraping and NLP with Requests, BeautifulSoup, and spaCy

Complete the tasks in the Python Notebook in this repository.
Make sure to add and push the pkl or text file of your scraped html (this is specified in the notebook)

## Rubric

* (Question 1) Article html stored in separate file that is committed and pushed: 1 pt
* (Question 2) Article text is correct: 1 pt
* (Question 3) Correct (or equivalent in the case of multiple tokens with same frequency) tokens printed: 1 pt
* (Question 4) Correct (or equivalent in the case of multiple lemmas with same frequency) lemmas printed: 1 pt
* (Question 5) Correct scores for first sentence printed: 2 pts (1 / function)
* (Question 6) Histogram shown with appropriate labelling: 1 pt
* (Question 7) Histogram shown with appropriate labelling: 1 pt
* (Question 8) Thoughtful answer provided: 1 pt

## Set Up

Create and Manage your Project Virtual Environment
This project uses external packages, which are not included in the Python Standard Library - we must install them. To keep our project separate from all other Python projects, we will create and manage a local project virtual environment. Additional details and commands are listed below.

Recommended Process
Open your project folder in VS Code.
Open a terminal window in VS Code (PowerShell for Windows, zsh or bash for Mac/Linux).
In the terminal, run the command git pull first, to make sure you have the current project contents on your machine.
In the terminal, run the command py -m venv .venv to create a new .venv environment in the project repo.
In the terminal, activate your environment using the command for your operating system.
In the terminal, use py -m pip install command(s) to install necessary packages into your active project virtual environment.
Edit your README.md to record your commands, process, and notes.
Set your VS Code Python Interpreter so your installed packages will be available for import.
In the terminal, run git add . then git commit -m "msg", then git push -u origin main to add / commit / push to GitHub.
Verify your GitHub repository.
1. Open Project Folder in VS Code
Open the project folder on your machine (the one you cloned from GitHub into your Documents folder) if not already open.

2. Open VS Code Terminal
Open a terminal window in VS Code (PowerShell for Windows, zsh or bash for Mac/Linux).

3. Git Pull
In the terminal, run git pull to fetch any changes that might have been made to the GitHub version. There may not be any changes, but it's good practice to pull every time you start work on a git project.

git pull
4. Create Project Virtual Environment (One-Time Only)
Use your terminal to create your project virtual environment by running venv as a Python module (py -m venv) and providing a name to use for the local folder as .venv. If you name it differently, be sure that your folder name is included in the .gitignore file.

Windows command

py -m venv .venv
Mac/Linux command

python3 -m venv .venv
You should get a new folder in your project repository named .venv. If VS Code asks to use use this environment, click Yes.

5. Activate the Project Virtual Environment (Every time you open a terminal)
Use your terminal to activate your project virtual environment. (Do this every time you open a new terminal to work on your project.)

Windows commands to activate your .venv. Try the first. Use the second if the first doesn't work.

.venv\Scripts\Activate
.\.venv\Scripts\Activate.ps1
Mac/Linux command to activate your .venv

source .venv/bin/activate
Verify you see the virtual environment name (.venv) in your terminal prompt.

6. Install Packages into Active Environment (One-Time, As Needed)
Verify your project virtual environment located in .venv is active. If not, activate it. You should see .venv in your terminal prompt. Use your favorite method to install the necessary packages.

At this point, the only project dependencies we know we need are:

requests - one of the most popular and widely used packages for web (HTTP) requests in Python
Windows command to install project dependencies:

py -m pip install jupyterlab pandas pyarrow matplotlib seaborn
Mac/Linux command to install project dependencies:

python3 -m pip install jupyterlab pandas pyarrow matplotlib seaborn
OR: Use requirements.txt to install packages instead

If you like, you can use a requirements.txt file to install dependencies instead. These files are helpful in projects when we have several external packages to install and it can be good practice.

To do so, you'll need a file named requirements.txt in the root folder of your repository listing each external package used, one per line.

If using Windows PowerShell, install into your active project virtual environment with this command:

py -m pip install -r requirements.txt
If using Mac or Linux, install into your active project virtual environment with this command:

python3 -m pip install -r requirements.txt
If successful, you will now be able to use the following line in your Python scripts. If you get an error on this line, work through the steps above to create, activate, and install into your local project virtual environment, and make sure VS Code is using your .venv local project environment.

import requests
