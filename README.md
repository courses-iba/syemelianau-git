## Work with repository workflow steps

##### 1. Clone repository (if haven't cloned yet):

```
git clone ssh://<username>@gml-jbpm.gomel.iba.by:29418/<username>-<course_name>
```
Ex.
```
git clone ssh://vpupkin@gml-jbpm.gomel.iba.by:29418/vpupkin-git
```

##### 2. Install commit-msg hook (if haven't installed yet):

```
<git\usr\bin>scp.exe -p -P 29418 <username>@gml-jbpm.gomel.iba.by:hooks/commit-msg <username>-<course_name>/.git/hooks/commit-msg
```
Ex.
```
<git\usr\bin>scp.exe -p -P 29418 vpupkin@gml-jbpm.gomel.iba.by:hooks/commit-msg vpupkin-git/.git/hooks/commit-msg
```

##### 3. When you're ready to start working on new task, create a new remote branch via gerrit based on master (if needed):

```
ssh -p 29418 <username>@gml-jbpm.gomel.iba.by gerrit create-branch <repo> <new-branch-name> master
```
Ex.
```
ssh -p 29418 vpupkin@gml-jbpm.gomel.iba.by gerrit create-branch vpupkin-git doc-gerrit-wf master
```

** Creating a new branch is the specific step to simulate team working on real project - new branch becomes your DEVELOPMENT environment with feature branch(es), master branch - is your PRODUCTION where only reviewed changes are allowed to be pushed. **

##### 4. Update your local repository from remote and now you're able to switch to the new local branch right away:

```
git fetch
git checkout <new-branch-name>
```

... Work on your task in this branch ...

##### 5. Add and commit your changes:

```
git add
git commit
```

** Just to have it well-formatted, please use following format template for commit messages: **

    courseName - taskNumber - detailedComments

** Remember to pull updates from remote master regularly **
** To add file to previous commit use --amend option **
** As you're the only person updating this repo - there shouldn't be any changes. But still, you should make this habbit appear, as your tutor can interfere and put some changes into master branch on his own, so make sure such cases are handled :) **

```
git checkout master
git pull origin master
git checkout <branch-name>
git merge master
```

##### 6. Push your changes into corresponding newly created remote branch (```refs/for/<branch-name>```) for review:

```
git push origin HEAD:refs/for/<branch-name>
```
Ex.
```
git push origin HEAD:refs/for/doc-gerrit-wf
```

... Wait for your Tutor to complete Verify and Code Review steps in Gerrit ...

##### 7. Retrieve latest changes from master (Remember? Tutor could make changes there):

```
git checkout master
git pull
```

##### 8. Merge your changes into master

```
git merge <branch-name> --no-ff
```

**--no-ff flag forces creating merge commit even if fast-forward merge is available.**

Ex. 
```
git merge doc-gerrit-wf --no-ff
```

##### 9. Push your changes into Gerrit (```refs/for/master```) for review:

```
git push origin HEAD:refs/for/<branch-name>
```

Ex.
```
git push origin HEAD:refs/for/master
```

... Wait for your Tutor to complete Verify and Code Review steps in Gerrit ... 

Once done, current task is completed. Congratulations! You can work on the next one.