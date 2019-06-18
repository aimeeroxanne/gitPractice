# GithubCollaboration

Tonight's class is a self-paced introduction to Git and Github. It will require you to do a lot of your own research, and thoroughly read the resources you encounter. This is the same way we teach our immersive programs to empower students to become independent learners.

**A few things to remember when you get stuck:**
- Have you googled it? 
- Can you communicate your problem effectively?
- Have you asked another student in class? 
- I am here for you after you've done all of the above. 

### What the heck is git? 

Git is a free and open source **distributed** version control system. Basically git is a software that you install on your computer to track the changes you make to a project for both individuals and teams. 

Lot's of programs have version control built in, like Microsoft Word or Adobe Photoshop. Version control essentially creates a history of your operations so you can "undo" them. Git is just like this only a little more complex. Unlike Photoshop and Word that save every action we take, with git we decide when to take "snapshots" of our work. These snapshots form a timeline that we can navigate. 

The **distributed** part is what allows us to collaborate with other developers. Basically each team member has their owen timeline and takes their own snapshots. As a team of developers, we each have our own 'version' of the project that we can periodically 'merge' with the master 'repository'. So, we have one single source of truth (the most perfect, up-to-date version of our project) on Github, and we each have our own 'version' of that project on our personal machines.  

### Ok, but then what is Github? 

Github, is equal parts cloud service, collaboration platform and social networking site. It's where developers of all kinds share their work, get noticed, and find open source projects they want to work on. 

It also provides the collaboration piece to git software described above. Think google drive but for developers, where our teammates can only see our changes when we say so. It's where we keep the 'master' version of our project, AKA the single source of truth, AKA the most up-to-date version of our projects. 

### Local vs. Remote...
Github is the remote. It's the folder in the sky, on the interwebz etc. Your local repository is on your computer, and your partners local repository is on their computer. Typically, in a team environment, there is one remote, and many local repos. This is not always the case, but for now let's move forward with that assumption.

### Adding, staging, commiting, pushing...


## Let's do this! 

**Setup**
- [ ] Install git on your machine: [for mac](https://desktop.github.com/), [for everyone else](https://git-scm.com/)
- [ ] Create a github account
- [ ] Instal a code editor: [Visual Studio Code](https://code.visualstudio.com/), [Atom](https://atom.io/), [Sublime](https://www.sublimetext.com/)
- [ ] Install your code editor of choice's Command Line Interface or CLI (Basically a speical set of commands that work with your editor) 

**Create a repo from the command line** 
The following will be done entirely via the command line, later we will add what is called a 'remote', an online version of our project on Github. For every command you don't know, do some research and create your own set of notes. 

- [ ] Open your terminal program
- [ ] Navigate to a folder where you want to work for the night
- [ ] Create a new folder `mkdir gitPractice`
- [ ] cd into that folder `cd gitPractice`
- [ ] List all the files in this folder, including the hidden files `ls -a` 
- [ ] Notice there is no .git folder
- [ ] Initialize a git repository `git init`
- [ ] List all the files in this folder, including the hidden files `ls -a`
- [ ] Notice there is now a .git folder. It is responsible for tracking all the changes in this folder. 

**Create a remote Github Repository**
- [ ] Login to Github
- [ ] In the top right corner, click the + icon and select 'New repository'
- [ ] In the 'Repository name' field, enter 'gitPractice' (Your 'remote' repository on Github does not have to have the same name as your 'local' repository but it will make your life easier.)
- [ ] Leave everything else the way it is and click the green 'Create repository' button 
- [ ] On the next page, copy the commands under the section where it says "...or push an exisiting repository from the command line"


**Add your newly created remote to your local repo**
- [ ] Paste the copied commands into your command line in the gitPractice folder, and hit enter. 
- [ ] You have just added a 'remote' to your 'local' repository

**Create some files that will be tracked**
- [ ] Create a file called readme.md in your repo `touch readme.md`
- [ ] From the command line, open the readme.md file with your text editor. (If you use VS Code, and have properly installed the CLI, the command is `code readme.md`)
- [ ] Add some markdown to your readme.md file! If you don't know what markdown is, google it!  


**If you already know the stuff above, and want to work on feature branch workflow...***

Partner A
- [ ] Create a repo from the command line and set up a remote on Github
- [ ] Add partner B as a collaborator

Partner B
- [ ] Clone the repo from Partner A
- [ ] Add index.html
- [ ] Commit
- [ ] Push

Partner A
- [ ] Pull down changes from Partner B

**Conflicts arise...**

Both partners:

- [ ] Create a branch (git checkout -b)
- [ ] Add an index.html file and a line of html
- [ ] Commit
- [ ] Push to your branch (git push origin branchname)

**Part 3 - Create a pull request**
- [ ] Read [the GitHub guide](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/)

Both partners:
- [ ] On the same screen, create pull requests to compare your branches with the master branch
- [ ] Analyze conflicts, if it's all good merge with Master
- [ ] Pull changes to your branch from master (git pull origin master)
- [ ] Switch to the master branch (git checkout master)
- [ ] Pull changes from master to your local master branch 
