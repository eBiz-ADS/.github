# Git Formatting
>_Please do follow the following format for readability and easier backtracking of issues._

#### Branch Name
>_Remove the brackets [] and replace the content inside with your actual branch name._

```
git branch [dev/module]

****Issue no. can be found on the project board when an issue is created.

Example:

git branch dev_login
```

#### Commit
>_Remove the brackets [] and replace the content inside with your actual commit message._

```
git commit -m "[fix/update/create/remove_issueorfeature#issueno_module--function/fix_versionoftheday]"

Example:

git commit -m "update_login--sessiontimeout_1"
```

>_If multiple modules, follow the format for readability._

```
git commit -m "[fix/update/create/remove_issueorfeature--whatdidyoufix/fix_versionoftheday]"

Example:

git commit -m "update_login|registration--sessiontimeout_1"
```


#### Pull Request Description/Comment

>_Remove the brackets [] and replace the content inside with your actual message._

```
Pull Request Title: [Repository Name--fix/update/create/remove module#function]

Example:

Pull Request Title: Alapaan v1--fix login--create user

Issue: [what features/functions]
Fix: [description on how the issue was fixed]
    - Fix 1
    - Fix 1
New: [if there are new features added]
    - Feature 1
    - Feature 2
Screenshot (optional): [what has changed]
```
