# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to `~/insy6500/class_repo`.
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git branch -M main` to establish a branch to push
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: ...
- Output of `git remote -v`:
- The output of `git log --oneline`:


### Reflections
#### Question 1:
a.) Before this assignment, I typically managed versions of my work using the file name. Git is more much more involved to set up than my previous method, however, it is far more powerful. Git offers commit messages, collaboration with others,
and the ability to merge work done in different parts.
b.) At previous jobs, I have written programs that automate various tasks, and thus exist outside of the main repositories used for production code. However, had I been able to access Git for these tools, I would have been able to version each iteration of the
tools, and would ahve been able to tag each update with rich version messages, allowing a new file associated with version for each use of the tool.

#### Question 2:
a.) It is important to keep the two repositories seperate, because there may be things in one repo that are named the same as the other repo. Pushing changes to a repo with a name that appears in another repo would overwrite files, which could
lead to data loss.
b.) For future coursework or projects, multiple repositories can be organized using descriptive names, paired with a descriptive README file. A group project would need to be shared with others, and thus, a public repository. While a 
repository of individual assignements and reference materials could be kept private.

#### Question 3:
a.) The commit message "update" is not a descriptive commit message, while "Add hw3a solution documenting Git workflow and repository structure” tells you much more about what was done between this commit and last. Suppose you had some sort of
accident in your repository and wanted to go back and see when the repository was last in its healthy state. Descriptive commit messages would allow you to recall loosly what each commit was, and where you should roll the repo back to.

b.) I believe that the best "unit of work" for a single commit is any time a new file is added or a file becomes functional. For example, if I add a data set to my repo, that can be committed without additional action. However,
if I have a preexisting Python file in this same repo, it would not be wise to commit it if it is not functioning as intended, relative to its maturity. That is to say that if I added a function in this file, it can be committed.
However, if this function is not complete, and has a bug that is being worked out, it should not be committed. The most logical "unit of work", in this sense, is any amount of work that behaves as intended, and keeps data
persistently iterated upon, which is beneficial especially in collaborative environments.


### Graduate Questions
#### Question 1:
a.) By committing the README and gitignore together, and committing the homework solution later, I was able to logically seperate commits to the repo. Since README and gitignore are more or less used in each repo, I was able to commit those as an
initial commit. By committing the homework solution later, I was able to seperate administrative changes from real content changes later on. The first commit gave me a solid building block to continue building my repo on.

b.) I would commit the README update, the typo, and the code used to load the data. The README tells the user what a repo is, so changes to that need to be kept current. The code used to load the data is presumably finished, and therefore can be
committed to the repo to keep the codebase current. I also commit the fixed typo because committed elements in a repo should be kept current to what is correct. The half-finished function can be committed at a later date once it is finished. It
is not very helpful to have half-finished code in a repository. Staging allows you to make this decision by git add only the files that you are ready to commit to the repo.

c.) git status allows you to make decisions about what to stage and commit by showing you files that have been added, modified, and removed. This allows you to add files that you wish to add to be committed in a more informed manner. This command
should be used in the workflow once you are ready to make a commit to the repo, but have not yet added files to staging.

#### Question 2:
a.) Git is a distributed version control system because an entire given repository and its version history can be pulled down to a local computer. This is different than storing files on Google Drive or Dropbox, because Git tracks the changes to files
and not just the files themselves. Git users also have access to files as they existed accross the repo history. Furthermore, using Git, users make changes locally, even while offline, and push them to the server. Conversely, Google Drive documents live
server-side, and thus changes must be made server side as well.

b.) The Git architecture allows collaboration to occur even while users are offline. This enables workflows wherein a user can take work with them to remote locations, planes, or even a location where internet access is simply not operational
at that time, and commit the changes at a later date, when connectivity is reestablished.

c.) `git clone` copies a remote repository to your local file system. `git pull` grabs the latest content from that remote location and merges it with your local instance of that repository. `git push` sends changes committed to the repository
to the remote location at which the repository is kept. class\_repo can be pulled from to merge to local changes. However, it cannot be pushed to, since it has permission limits set by the professor. my\_repo allows both because I am the originator of the repo
with full permissions.

#### Question 3:
a.) When deciding what to commit, it is best to consider if the files to be committed serve their intended purpose as-is. In order to balance showing the working process, versus presenting final projects, descriptive commit messages are a _must_.
These commit messages can contain information letting another user know what is finalized, versus still in-work. To show the working process, more frequent smaller commits may be wise, paired with descriptive messages to explain increments.
Before submitting a polsihed product however, fewer larger commits may be desired with commit messages reflecting that a given commit is a major update to a polished state.

b.) A README for a portfolio should provide information about what the portfolio contains to include structure, types of work, and languages. A README for an open-source project that others may use should contain documentation on the same sorts of
information, with the addition of _how_ to use the repository. This could include information on how to build/compile the code, dependencies, hardware reccomendations, example code snippets, etc.. In the case of the portfolio, the README should
describe what the repo is, and what it contains, while the open source code README should contain what the repo is, what it contains, _and_ how to use it.

c.) Building this public portfolio _during_ coursework, as opposed to during job searches, allows a rich commit history of the repository to be developed. At its deepest point, such history shows the process of learning, and growth, which are
valuable traits to a prospective employer. In order to make this portfolio valuable later, good habits to practice are frequent commits with descriptive messages, descriptive README file to help other users understand the skills you are trying
to display with each project, and complete commits that contain functional blocks of work.
