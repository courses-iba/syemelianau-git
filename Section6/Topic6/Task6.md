## Task 6 Rebase, take it easy.

** You should perform operations using Command Line processor / Git Bash only! **

#### Follow the next steps to achieve the task completion:

Preparation Steps:

1.  Create and go to branch *Section6* on basis of branch *master* on server and pull changes to local;
2.  On local create branch *Section6r* on basis of branch *Section6* and go to it.
2.  On branch *master* create a new file *Section6/rebase_msample.txt* and set several lines of text there;
3.  Commit your changes with message "Rebase source" and merge updates to branch *Section6r*;
4.  On branch *master* put some more updates to the same lines and commit changes with message "Master Rebase 2".
5.  On branch *master* put some more updates to the same lines and commit changes with message "Master Rebase 3".
6.  On branch *Section6r* add a new file *Section6/rebase_fsample.txt* and set several lines of text there;
7.  Put some more updates to the same lines and commit changes with message "Feature Rebase 2".
8.  Put some more updates to the same lines and commit changes with message "Feature Rebase 3".

Tasks:

9.  Rebase changes from branch *master* to branch *Section6r* - no conflicts should appear.
10. On branch *Section6r* put some more updates to the *Section6/rebase_msample.txt* file and commit changes with message "Feature Rebase 4 conflicts".
11. Get on branch *master* and put some more updates to *Section6/rebase_msample.txt* file - text should differ on the same lines between branches *master* and *Section6r*.
12. Commit your changes with message "Master Rebase 4 conflicts";
13. Rebase changes from branch *master* to branch *Section6r* - abort conflicts and then rebase again to resolve conflicts(using rebase, not merge!).
14. Merge changes from branch *Section6r* to branch *Section6*;
15. Get this file (Topic6/Task6.md from branch *Tasks*) included to latest commit of branch *Section6* using amend option;
    Push commit to corresponding server branch for a review;

Final Steps - merge all to master branch:

16. Once reviewed by Tutor, merge all the changes to branch *master* (Check README.md file for instructions);
17. Change to branch *master* if not yet on it;
18. In directory *Section6* run command *history >> history6.txt* and stage changes;
19.	Include these changes into previous commit (Check README.md file for instructions);
20.	Push branch *master* changes to server for review;
21. Once reviewed by Tutor, task is completed.

#### Once done, you can follow up on next Topic/Task assignment.