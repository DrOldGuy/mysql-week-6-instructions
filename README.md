# MySQL Week 6 Instructions

# About the assignment

This week's assignment is a collaborative MySQL/Java coding project. You need to think up a project that everyone can contribute to. It's a team project with a team grade. You may want to start thinking about this early because any collaborative project takes more time than you think it should. You will need to use git as the VCS (version control) for the entire project (think branches and pull requests).

Here are some possibilities:

* A person does the menu
* A person creates a service to assemble the data
* A person creates a DAO class
* One or more people write stored procedures for the data operations (CRUD)
* A person writes the DDL (SQL statements) to create the database and the tables
* A person tests and accepts the final code
* A person creates and uploads the project deliverables

Use your imagination! Here are some possibilities to get you started:

* Create an inventory application with vendor, parts and inventory tables
* Create a blog with members, posts, and comments
* Create a recipe app with recipe details, ingredient and step tables.

Or anything else you want!

Here's how I would approach this (if I were doing it):

1. Appoint a project manager. This person is responsible for coordinating all the workers and work done.
1. Come up with the general idea and get buy-in.
1. Design the operations (what, specifically will the app do - think "use cases").
1. Design the tables to support the operations.
1. Divvy up the work.
1. Implement and turn in.

**TODAY** would be a good day to get started on this - you only have a week.

Final thought: it's easy to come with a design that's so broad that you won't be able to do it in a week. Use your head.

## About the teams

Form teams of two or three people and post who's on what team. If someone asks to be on a team please play nice and let them in. Here's the class roster if you need it: Colin Cramer, Daisy Murillo, Jason Howard, Jess Raben, Kim Watson, Lee Blanchard, Zach Rind.

If you want, we can use Wednesday night's session to work on the assignments. Teams can work individually and I'll be available to ask questions. If you don't want to do that we can go over any topic learned so far so that you can ask questions.

## Working on the project

One person should create the team repo on GitHub. Set the repo visibility to public. You will find that if your team updates to the master branch that you will lose work. There's a better way.

1. Create the repo. Send the project URL to your team.
1. Open the project main page (Code) in a browser. Click on the big green "Code" button. Copy the clone URL.
1. Open a command window and nagivate to your workspace directory (the one in which your projects live). Type **git clone ** and paste the clone URL into the command line. Example: *git clone https://github.com/DrOldGuy/mysql-week-6-instructions.git*. This will create the project directory as a subdirectory under the current directory.
1. Open your IDE and enter the workspace. Right-click in a blank space in Project Explorer and click "New / Java Project". Enter the project name (the directory name of the project that was cloned). Click "Finish" then "Don't Create" if you are using Java 9+. Eclipse should create the project, and you should see the git branch in the project name. So, for project mysql-week-6-instructions, you should see in the Project Explorer "mysql-week-6-instructions [mysql-week-6-instructions master]", where "master" is the name of the master branch.
1. Make any changes you want.

## Push changes to GitHub

1. When done making changes open a command window and navigate to the project root directory (i.e., .../mysql-week-6-instructions): **cd <workspace>/mysql-week-6-instructions**.
1. Type **git status**. You should see the changed files in red.
1. Type **git add .**.
1. Type **git status** again. You should see the changed files in green.
1. Type **git commit -m "Some comment"**.
1. Type **git push origin master:A_Branch_Name** where "A_Branch_Name" is the name of a branch to create in git. It's good to put your name and the short branch name like this: **git push origin master:rhewitt_added_service_layer**. There must be no spaces in the branch name or before and after the colon. This will create the branch locally and remotely but you will still have the master branch checked out locally. That's OK.

## Create a pull request

Next create a pull request in GitHub. This will allow the changes to be *merged* into the master branch instead of overwriting the master branch. Muy importante.

1. Navigate to the project URL with a brower. You should see a big green button "Compare & pull request". Click the button.
1. Add reviewers if you want. Otherwise click the big green "Create pull request" button. You may need to be the repo creator for this.
1. Go to the "Pull requests" tab. (You should be on it if you just clicked "Create pull request". Click the "Merge pull request" button. Click "Confirm merge". You may need to be the repo creator to do this.
1. Go back to the Code tab. You should see your changes merged into the master branch.
