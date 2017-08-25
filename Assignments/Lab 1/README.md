# Lab 1: Hello Professor

This assignment involves: 
1) getting your toolchain set up and tested; 
2) creating a "Hello Professor" application to introduce you;
3) submitting a resume and cover letter.

## Toolchain
A "toolchain" is the set of tools you use to build and test and application. For now, this will include g++, CodeLite and GitHub.

### G++
g++ is the Gnu C++ compiler. It is already installed and ready to go on the lab machines. 

#### Windows
On Windows, you want to install TDM-GCC. You can download the installer at http://tdm-gcc.tdragon.net/.

#### Mac
On Mac, open the "Terminal" application. At the command line, type "g++". Your Mac will recognize that g++ is not installed, and walk you through the installation process.

#### Linux
Installing g++ is easy on Linux, but the details will vary based on what distribution you are using.
In most cases, you want to install either "gcc" or "gcc6".

### CodeLite
CodeLite is already installed on the lab machines. You can also download it for your own computer at http://codelite.org.

When you first start up CodeLite, it will walk you through a wizard to help you get it configured the way you want it. 

After going through the wizard, create a workspace for this course. Most students use "files/csc319" as the workspace on the lab machines. 

### GitHub
Sign up for a GitHub education account, which will allow you to have private repositories, suitable for classwork. You also get access
to free resources at many other companies as part of the program. Get details and sign up at https://education.github.com/pack.

## Hello Professor application
1) Accept the assignment. Got to https://classroom.github.com/a/f68vNb6M and accept the assignment. This will create a private GitHub repository where you can work on the assignment. Copy the URL of the repository to your clipboard.
2) Clone the repository to your workspace. In CodeLight there is a tab at the bottom for "Git." Click this tab, then click the icon at the far left "Clone a Git Repository." Paste in the URL for your repository into "Clone URL," adding ".git" at the end if it isn't already there. Browse for the "Target Directory" and select your CodeLight workspace (typically "files/csc319" unless you picked something else).
3) Switch CodeLight to use the Git Repository. Click the icon on the far right "Set repository path" and then browse to the Lab 1 repository, something like "files/csc319/lab-1-username."
4) Create a new project. For the type of project, under "Console" pick "Simple executable (g++)." Name the project "Lab1" and check the box
for "Create the project under a separate directory." The default values for the toolchain should be correct.
5) You need to tweak the compiler settings. CodeLite provides a project browser in a pane on the left. 
Right-click the name of the project ("Lab1") and choose "Settings" and then "Global Settings."
- C++ Compiler Options: Click the "..." on the right and choose: -Wall, -std=c++11, -O0, -g, -pedantic-errors.
- C Compiler Options: -Wall, -std=c99, -O0, -g, -pedantic-errors.
6) Link your project to Git. Click the "Git" tab at the bottom of the window. 
7) Build the sample application. CodeLite made a basic "Hello World" application for you. To compile it and run it,click "Run" in the "Build" menu.
8) Replace the application code. Click the ">" to the left of the project name. Navigate into "src" and click on "main.cpp." Replace the sample C code with proper C++ code.
