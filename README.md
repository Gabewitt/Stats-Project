## Working with Git command lines

There are some specific command lines that you need to know to make collaborating easier for everyone.

### Pulling

Before starting to code on a lovely sunny day, perform:

`git pull`

which will pull the most recently updated version of the code from github.

This would how you update the notebooks from other people.


### Git branches


Github uses a system called **Branches**. The original, and public (sharable) code is located on the **Main Branch** (one can see which branch they are on by looking at the bottom left of their VScode window). 

It is very important to not mess/change code while inside the **Main Branch**. If you want to tweak, or create a new function, you need to create a new branch or go into an already existing one if there is.

`git branch NameOfBranch`

To make it easier for everyone to follow, **NameOfBranch** should follow this format:\

*git branch gwitt/1712_worked_on_q1*
*git branch gwitt/2012_woked_on_q1_a*

Once the branch is created, you need to access the branch.

`git checkout BranchName`

Example:

*git checkout gwitt/1712_worked_on_q1*
*git checkout gwitt/2012_woked_on_q1_a*

Once in the branch you are free to change the code/create new files...



### Pushing your code

Now that you've finished with your code for the day and before going out with your friends to go drink, you should load your code into the github repository for you colleagues to see and access.

You can see what has or hasnt been updated to the main branch by running:

`git status`

To upload your code. This is done in three steps.

First you need to add your code, or Stage your code.

`git add NameOfFile`

Where NameOfFile are the code files you want to update. If you want to update all the files at once:

`git add .`

Now you need to commit the changes.

`git commit -m "Message"`

Be sure as the message, to indicate what you did, for other people to read such as:

*git commit -m "Commitment Issues"*

Finally, you need to push the data towards github.

`git push`

This might prompt an error code in the terminal if you are uploading your branch for the first time. The error code will provide you with a new command line to run. Be sure to run that.

Congrats, you have just updated our github repository. Well almost.


**VERY IMPORTANT**

You can see how many changes you have made when you click the repository icon on the left sidebar of vscode. Initially after downloading all the packages, you might have hundreds of changes. You do not want to upload whole packages as everyone already has them installed. So select all the changes by doing cammand+A, then right click and there should be an option to **Add to gitignore**. And be sure to do so. Then you can commit and push that gitignore file afterwards.


## Conforming the changes on the GitHub website


Once on the github website, you should see a new message above the repository where it says **Push Request**. This happens because someone needs to approve your code before it goes into the main branch. Follow the steps indicated, and someone will get a message to approve it. 

I will try and change that and make sure you dont need to wait for someone to do it. This feature is to stop bad coders uploading shit to the repository.


Now you are done ! 

Back on vscode, you can go back into the main branch, by clicking the branch icon at the bottom left corner of the window, and choose main again. To check that everything is fine, perform a `git pull`.
