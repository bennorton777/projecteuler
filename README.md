# projecteuler

From the site:
"Project Euler is a series of challenging mathematical/computer programming problems that will require more than just mathematical insights to solve."
https://projecteuler.net/about

This repository is for the discussion of these problems.

# git instructions

You'll need git to interact with the repository.
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

To submit content to the repository, begin by cloning the project:
```
git clone https://github.com/bennorton777/projecteuler.git
```

When you clone the project, you'll be on the _master_ branch.  The process for adding content to this repository is to:

Update your local master branch by first making sure you're on the master branch (you'll begin by default there when you first clone the project):
```
git checkout master
```
and then "pulling" (updating) master:
```
git pull
```
Making a new branch:
```
git branch my-kickass-branch
```
Switching to that branch:
```
git checkout my-kickass-branch
```
Adding content to the appropriate problems folder (make a new one if the one you want isn't already there) using whatever program or utility you please:
```
 some process by which I add directory:
 problems/42/
 and file:
 problems/42/recursive_solution.rb
```
Adding your files to the staging area.  The staging area is just a collection of files that you intend to commit.  If there were no staging area, committing would just commit everything you've changed in the repository every time, which isn't necessarily if you want.  It may make sense to make two separate commits for your work on two separate problems.  Add the files to the staging area with:
```
git add problems/42
```
Committing the changed files in your staging area:
```
 git commit
 (add a message to the top line of the editor.  It will probably be vim by default.)
```
Pushing your local branch + committing to the upstream repository on github:
```
git push origin my-kickass-branch
```
Time to submit your pull request!  Go to the github ui - it will very likely have a link for you asking if you want to "compare and make pull request."  If you don't see it, you can select my-kickass-branch from the dropdown menu next to the repository name, and click the pull request button on the right hand side above the latest commit message.

At this point you'll be presented with a graphical representation of a diff.  You haven't actually made a pull request yet, you're looking at the diff to see if it looks good.  If you're satisfied with your diff, you can use the create pull request button!  Once this has happened, collaborators can make comments on lines in your diff, and you can discuss the solution.
 
If at any point you want to make an update to your pull request, simply go back to the "Adding content" step, and repeat through pushing to your branch.  When the discussion of your submission is concluded, the merge pull request button can be used to add the new commits from your branch to upstream master.  The next time someone pulls, your vetted commits will be on their local master.

