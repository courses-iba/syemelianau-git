## Task 7 The Golden Rule of Rebasing

** You should perform operations using Command Line processor / Git Bash only! **

#### Follow the next steps to achieve the task completion:

Preparation Steps:

1.  On branch *master* update *Section6/rebase_msample.txt* file on several lines of text there;
2.  Commit your changes with message "Master of Golden Rule";
3.  On branch *Section6* update *Section6/rebase_msample.txt* file on several lines(same lines as before) of text there;
4.  Commit your changes with message "Feature of Golden Rule";

Tasks:

5.  Rebase changes from branch *master* to branch *Section6* (Section6 is prioritized) and resolve conflicts if needed (using rebase, not merge!);
6.  Get this file (Topic6/Task7.md from branch *Tasks*) included to latest commit of branch *Section6* using amend option;
7.  Push commit directly to corresponding server branch (do not use HEAD:refs/for/).
8.	Since you have recieved an error message about updates being rejected because the tip of the current branch is behind its remote counterpart -
    Read about the Golden Rule of Rebasing, (for example, from here: https://habr.com/company/otus/blog/352640/ ), 
    then undo the rebasing and fix your local branch, then resend it for a review (No push-force allowed).

Final Steps - merge all to master branch:

10. Once reviewed by Tutor, merge all the changes to branch *master* (Check README.md file for instructions);
11. Change to branch *master* if not yet on it;
12. In directory *Section6* run command *history >> history7.txt* and stage changes;
13.	Include these changes into previous commit (Check README.md file for instructions);
14.	Push branch *master* changes to server for review;
15. Once reviewed by Tutor, task is completed.

#### Once done, you can follow up on next Topic/Task assignment.