# Lab 1: Hello Professor

This assignment involves: 
1) getting your toolchain set up and tested; 
2) creating a "Hello Professor" application to introduce you;
3) submitting a resume and cover letter.

* This is an individual assignment. *
You may help each other figure out how to get the tools set up and working, but you are responsible for writing the application code, resume and cover letter yourself. If you use a resource to help you write the application, you should provide a reference to the resource in a comment in the code. For this assignment, the textbook is a useful resource.

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
4) Create a new project. For the type of project, under "Console" pick "Simple executable (g++)." Name the project "Lab1". Browse to the path for the lab, something like "files/csc319/lab-1-username." If it is checked, clear (uncheck) the box
for "Create the project under a separate directory." The default values for the toolchain should be correct.
5) Commit the clean initial project to Git in case anything goes wrong. Drag the Git box a little larger so you can see the content, if necessary. On the left, there should be a list of files with "untracked changes." Click on each file in turn, then click the "Add File" icon near the left end of the Git icons. Once every file has been added, click the "Commit local changes" icon. Enter the message "Initial version" and commit.
6) You need to tweak the compiler settings. CodeLite provides a project browser in a pane on the left. 
Right-click the name of the project ("Lab1") and choose "Settings" and then "Global Settings."
- C++ Compiler Options: Click the "..." on the right and choose: -Wall, -std=c++11, -O0, -g, -pedantic-errors.
- C Compiler Options: -Wall, -std=c99, -O0, -g, -pedantic-errors.
7) Build the sample application. CodeLite made a basic "Hello World" application for you. To compile it and run it,click "Run" in the "Build" menu.
8) Replace the application code. Click the ">" to the left of the project name. Navigate into "src" and click on "main.cpp." Replace the sample C code with proper C++ code. Commit the change to GitHub and then make sure it runs OK.
9) Modify the program so that it introduces you to the professor and tells him something interesting about yourself. Commit the change to GitHub and then make sure it runs OK.

## Resume and Cover Letter

Make a resume or update your current resume. Also make a cover letter that is specific to this course. The cover letter should:
1) Contain any keywords found in the job ad that are not present in your resume, even if you have to say something like "I have never used a compiler before, but I learn quickly and look forward to using one."  In this case, use the syllabus as if it were a job ad.
2) Make it clear that you know what the job is and that you are excited by it.
3) Explain in what ways you can contribute value to the company if you are given this job. Said anather way, explain why you are a good candidate for this position.
4) Mention that you will provide references on request. They should not be listed on your resume, and you should rarely include them in the cover letter.

Place the resume and cover letter in your "lab-1-username" directory and commit them to GitHub.

# Grading

Assignments will only be accepted through GitHub.

- (5 pts) Initial commit exactly as CodeLite created the project before you made any changes.
- (5 pts) A commit with a "Hello world" application in proper C++ (not in C).
- (5 pts) Final commit compiles with no warnings.
- (5 pts) Final commit is in C++ (not C) with good style, comments, etc.
- (5 pts) The output of the final commit introduces you to the professor. (Example: "Hi, Steven. I am John Doe.")
- (5 pts) The output of the final commit says somethinng interesting about you.
- (30 pts) An up-to-date resume is submitted.
- (10 pts) The cover letter contains keywords from the sylabus.
- (10 pts) The cover letter makes it clear you know what the class is about and are excited to be in it.
- (10 pts) The cover letter says what you can contribute to make the classroom experience better for the whole class.

The resume and cover letter will be accepted late with a penalty of 5 pts each. Late submissions should be turned in via email. The program code will not be accepted late.
