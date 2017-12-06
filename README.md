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

