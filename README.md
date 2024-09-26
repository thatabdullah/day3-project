1.firstly i created a folder called project inside my bootcamp's workspace
    mkdir project
    cd project
    git init tasks-manager

2.then i created a text file with the tasks appointed in the project's PDF then staged them and committed them
    git add .
    git commit -m "first two tasks added"

3.after that i created a branch called feature/add-tasks, i missnamed the branch name so i used "git branch -m (oldname) (newname)"
    git checkout -b feature/add-tasks
    echo "- practice git branching" >> tasks.txt
    git add .
    git commit -m "third task added"
    
3c&d.i created a new branch named feautre/remove-tasks then deleted a task in and committed it
    git add .
    git commit -m "a task removed"

4.i moved to the master and did a fast-forward merge successfully
    git checkout master
    git merge feature/add-tasks

b.when i tried to merge the second branch i faced a conflict and resolved it 
git merge feature/remove-tasks


5. i created a new branch then edited the text file
    git checkout -b feature/update-tasks
    echo "- Review Git merge and rebase" >> tasks.txt
   git add .
   git commit -m "updating task"
   

c. i switched to the master branch and rebased with the new branch
    git checkout master
    git rebase feature/update-tasks

7. i added an incorrect sentence to the text file then reverted it
     echo "xxxx" >> tasks.txt
     git add .
     git commit -m "incorrect statement"
     git revert HEAD

8. i did a reset command on a commit as requested
     git reset --hard 1c98d8ae2f112b4b01f1431b54e868fba15ede2e

9. i pushed it to the github repo

   
   
    

