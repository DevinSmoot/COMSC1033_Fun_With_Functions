# Read.Me file to start a program:
	Example: for fun with functions

1. Start Eclipse
2. Change the workspace to our thumbdrive
	: File->Switch Workspace
3. Start a new project: Fun_With_Functions_Project
	: File->New Project
		: Use default runtime environment,
			then click finish.
4. Add a new class with our new 
	project selected: Fun_With_Functions
	: File->New->Class
	: Name the project, select public static 
		void main option and click finish.



Now start Git and GitHub

1. Open a command prompt:
	: Start->search for cmd->Press Enter.
2. Go to your project folder:
	: E: to change to thumb drive.
	: dir to list the directory
	: E:\>cd Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project
	: E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project
	You should be able to see 
	the src and bin folders.
3. Define user information:
	: git config user.name "Devin Smoot"
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git config user.name "Devin Smoot"
	: git config user.email smootd@student.swosu.edu
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git config user.email smootd@student.swosu.edu
4. Initialize the project:	
	: git init
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git init
	Initialized empty Git repository in E:/Documents/School/Fall 2015/Computer Science 1/Workspace/COMSC1033_Fun_With_Functions_Project/.git/
5. Add current files:
	: git add .
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git add .
6. Commit current files and changes:
	: git commit -m "initial commit"
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git commit -m "initial commit"
	[master (root-commit) f3e497c] initial commit
	 4 files changed, 35 insertions(+)
	 create mode 100644 .classpath
	 create mode 100644 .project
	 create mode 100644 bin/Fun_With_Functions.class
	 create mode 100644 src/Fun_With_Functions.java
7. Go to GitHub and create a new repository:
	: http://github.com
	Log in to GitHub.com
	: https://github.com/login
	On the right side click: 
	: + New Repository
		: Enter repository name
		: Enter a description
		: DO NOT INITIALIZE
		Click: Create repository
8. Push current local repository to GitHub repository just created:
	Copy from GitHub:
	: git remote add origin https://github.com/DevinSmoot/COMSC1033_Fun_With_Functions.git
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git remote add origin https://github.com/DevinSmoot/COMSC1033_Fun_With_Functions.git
	: git push -u origin master
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git push -u origin master
	Paste to command line.
	Enter username and password for GitHub when requested on command line.
	Username for 'https://github.com': DevinSmoot
	Password for 'https://DevinSmoot@github.com':
	Counting objects: 8, done.
	Delta compression using up to 4 threads.
	Compressing objects: 100% (8/8), done.
	Writing objects: 100% (8/8), 1.16 KiB | 0 bytes/s, done.
	Total 8 (delta 0), reused 0 (delta 0)
	To https://github.com/DevinSmoot/COMSC1033_Fun_With_Functions.git
	 * [new branch]      master -> master
	Branch master set up to track remote branch master from origin.
9. Create a development branch:
	: git checkout -b dev
	E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project>git checkout -b dev
	Switched to a new branch 'dev'
10. Save markdown ReadMe.md file:
	: File->Save As
	Change directory to project folder
	: E:\Documents\School\Fall 2015\Computer Science 1\Workspace\COMSC1033_Fun_With_Functions_Project
	Change file extension to: All Files
	Filename is: ReadMe.md
11. Push changes to dev repository:
	Copy the repository url from GitHub on the right side:
	: https://github.com/DevinSmoot/COMSC1033_Fun_With_Functions.git
	Push ReadMe.md to GitHub (remote) repository:
	: git add .
	: git commit -m "Added ReadMe.md to repository"
	Set the remote branch to dev
	: git push --set-upstream origin dev
	