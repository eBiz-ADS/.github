
# Git Formatting
>_Please do follow the following format for readability and easier backtracking of issues and for automating our semantic versioning._

## Release Tag
**Dev Tag Releases**
> v0.0.1-dev.1

**Staging Tag Releases**
> v0.0.1-beta.1

**Production Tag Releases**
> v1.0.0

**Type of releases**

 1. **PATCH** in Semantic Versioning  
 2. **MINOR** in Semantic Versioning 
 3.  **MAJOR** in Semantic Versioning

**Categories**

-   **feat**: A new feature
-   **fix**: A bug fix
-   **docs**: Documentation only changes
-   **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
-   **refactor**: A code change that neither fixes a bug nor adds a feature
-   **perf**: A code change that improves performance
-   **test**: Adding missing tests
-   **build**: project build
-   **chore**: Changes to the build process or auxiliary tools and libraries such as documentation generation

## Branches

**Main Branches**
-   **master**: production
-   **dev**: development
-   **staging**: uat/staging

#### Branch Name (parent issue branch) (created by lead dev)
>_Remove the brackets [] and replace the content inside with your actual branch name._

```
git branch [create/update/fix]

****Issue no. can be found on the project board when an issue is created.

Example:

git branch create/userlogin
```
  

#### Branch Name (sub-issues branch)
>_Remove the brackets [] and replace the content inside with your actual branch name._

```
git branch [feature/enhancement/fix/style/build]

****Issue no. can be found on the project board when an issue is created.

Example:

git branch feature/login
```

#### Commit
>_Remove the brackets [] and replace the content inside with your actual commit message._

```
git commit -m "[fix/feat/perf/doc/build/style/refactor(optional scope): module description' ]"

Example:

git commit -m "feat: create login form for registration and login"
```
