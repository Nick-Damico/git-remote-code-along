Git Remotes and Github Codealong
499 STUDENTS COMPLETED

OBJECTIVES
Describe GitHub and its relationship with Git
Create a remote repository on GitHub
Use git push to connect your local repository of files to your remote repository
Use git remote
Use git push
Use git pull
Let's go through an example to clarify remote repositories on GitHub.
CREATE A LOCAL DIRECTORY
In your development directory, create a folder: mkdir git-remote-code-along.
Change directory: cd git-remote-code-along.
Add a README: touch README.md.
CREATING A REMOTE REPOSITORY ON GITHUB
Go to github.com/new.
After you create the repo, click the "Copy to clipboard" symbol on the right-hand side of the screen (GitHub clipboard) to copy the clone url (we'll use this in the next section).
CONNECTING YOUR REMOTE REPO TO A LOCAL REPO
git init.
git add . + git commit -m "initialize git". Add and commit the new file created by the git init command in step 1.
git remote add origin your-remote-repository-URL. This sets the remote, so you can push and pull code.
PUSH CODE TO GITHUB
Let's add something to our README. Open the file and add whatever text you'd like.
Now look at the remote repo on GitHub. Notice that the new text in your README is not there. Let's fix this by pushing our code up to GitHub.
If we git push right away, we still won't get the changes because we have not tracked and committed the changes. Let's do that: git add . and git commit -m "add content to README".
Now we can git push -u origin master. We only need to apply the -u flag (short for --set-upstream) the first time we use git push. It tells the current local branch to track itself against the master branch of origin, the remote repo we're pushing to. After you've set the upstream link with -u, you can use git push and git pull without specifying any arguments (such as a target branch or repo).
Confirm that your changes are now visible on GitHub, and you're done!
PULL CODE FROM GITHUB
git pull
This command takes any new changes to the remote repository and "pulls" them down to your local code. Try running it in your terminal now. In our case, there's nothing to pull, so you should see a message that says Already up-to-date.
Sometimes the code on your remote gets ahead of your local code. This happens often when collaborating with others, but it can also happen when you edit code directly on GitHub.com. Let's give that a try.
EDITING DIRECTLY ON GITHUB
Say you liked your README, but you noticed a minor typo. Let's fix it directly on GitHub.
Navigate to your remote repository on GitHub.com, e.g., https://github.com/username-here/repository-name-here.
Click on your README file.
At the top of the file, you'll notice a pencil icon (GitHub pencil). Clicking this will allow us to edit the file.
Make some changes to your README.
Commit them by clicking the "Commit changes" button at the bottom of the page.
Perfect! But now the code on our machine (in our local repo) is out of sync with the remote repo. To remedy this, we must pull down the code to our local repo. To do so, run:
git pull
 LEARN. LOVE. CODE.	TERMS & CONDITIONS	MADE WITH  BY FLATIRON SCHOOL


Ask a Question
Questions Need Help
Finish Reading
I'M DONE
NEXT LESSON
CREATE A STUDY GROUP
