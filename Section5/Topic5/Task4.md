## Task 4 Branches and Branches.

** You should perform operations using Command Line processor / Git Bash only! **

#### Follow the next steps to achieve the task completion:

Preparation Steps:

1.  Create and go to branch *Section5* on basis of branch *master* on server and pull changes to local;

Tasks:

2.  Create a new directory *Section5* and create file *newFile.txt* there, adding sample text 'Hello' on the 1st line of the file;
3.  Commit current changes; 
4.  Return to branch *master*. On basis of branch *master* create new branch *s5feature* on local;
5.	Merge branch *Section5* to branch *s5feature* with fast-forwarding option;
6.	Update *Section5/newFile.txt* - put sample text 'World' on the 2nd line of the file;
7.	Commit current changes;
8.	Get back to branch *Section5* and update *Section5/newFile.txt* - put sample text ', World!!!' on the 2nd line of the file;
9.	Commit current changes;
10.	Merge changes from branch *s5feature* without fast-forwarding option - use P4Merge Tool to resolve conflicts;
11.	Update *Section5/newFile.txt* - remove end line symbol on the 1st line of the file, it should now contain only 1 line with sample text 'Hello, World!!!';
12.	Get this file (Topic5/Task4.md from branch *Tasks*) to branch *Section5* to directory *Section5*;
13.	Commit latest change with amend option and push commit to corresponding server branch for a review;

Final Steps - merge all to master branch:

14.	Once reviewed by Tutor, merge all the changes to branch *master* (Check README.md file for instructions);
15.	Change to branch *master* if not yet on it;
16.	In directory *Section5* run command *history >> history4.txt* and stage changes;
17.	Include these changes into previous commit (Check README.md file for instructions);
18.	Push branch *master* changes to server for review;
19. Once reviewed by Tutor, task is completed.

#### Once done, you can follow up on next Topic/Task assignment.