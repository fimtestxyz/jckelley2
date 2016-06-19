This is a tutorial I follow to practise github 

1. git init 
2. git diff , git diff --staged
3. git add
4. git commit -m 'comment message'
   git commit --amend -m 'new commit message' ; this is useful when you just make a mistake when you commit. Assume that none of your team member just continue to build on top of the commit message, you can use this cmd
5. git hist , git sg (my own alias git log type of commands)
6. git branch , git branch -D  'branch id'
7. git co -- <filename> ; to get that <filename> from repository and overwrite the working copy of filename
8. git reset HEAD <filename> ; to un-stage the <filename> which you just 'git add'
9 a.) git reset --soft <commit id> ; this is useful when what to change your latest commit id message , your working copy is the latest copy one, and your staging is also the latest copy one
  b.)git reset --mixed <commit id> ; after running this cmd, your working copy is the latest copy one, your staging is the <commit id> copy
  c.) git reset --hard <commit id> ; this will go to commit id, all your working copy and staging will be over-written by <commit id> copy. Use this carefully
10. git tag -a v1.0 'this is v1.0' ; git co <commit id> first and then run this git tag cmd to label that with a tag, run 'git tag'  to see all the tags
