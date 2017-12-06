Before you start working on your project, make sue to pull the latest change from the repository

=> git pull origin master

After you made changes to your code
  1. check to see what files you edited that have not been tracked
  => git status (new changes are red)
  2. Add the new changes to the commit
  => git add . (make sure to use period where it is)
  3. Commit changes to repo with a message
  => git commit -m "Added new changes"
  4. Recheck status of new changes again
  => git status (new changes now should be green)
  5. Push new committed changes to repo
  => git push origin master (push to master branch)
  
In real world, you don't want to work with master branch (it can lead to conflicts)
For example, developer A should work with branch A. Developer B should work with branch B

To create your own branch A:
=> git checkout -b A

After execution of above command, it should give you a message "Now on branch A"
Now you can make your changes, which only reflect on branch A, not master
For example, add a new html file call a.html

Then do: git status => git add . => git commit -m "Added a.html"
Now you want to push to branch A only
 => git push origin A
 
Now you if you go and look at your repo on github, you can see that only branch A gets updated
Once you're happy with your new changes, you want to combine it with branch master by merging them together

First switch master branch if you're currently in A
=> git checkout master

Then merge master with A
=> git merge A

Push merged result to master
=> git push origin master

Now you if you go to look at master, it should be the same as A
You can delete branch A now if you do not wish to work with it anymore
=> git branch -d A

If you wish to continue working with branch A, switch to branch A now
=> git checkout A (note: no need to do -b)




