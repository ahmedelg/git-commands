# Links
## Git Merge
https://www.youtube.com/watch?v=74ZuPrgzRpE

لابد وأن يكون هناك فرع غير الافتراضي والرأيسي خاص بالتطوير 
بحيث ان الاساسي يكون خاص ب 
deployment
وجعل مع الفرع الكثير من الفروع كل فرع خاص ب 
feature معينة

- - -

## Git Course
### Git Architecture
https://www.youtube.com/watch?v=Q5Eb3jBvFEE&list=PL_aOZuct6oAogr4UMkWddU7leOXw0QKJS
1. Working directory > Project in device
> git add > `Staging Area` >Delete >Modify
> git checkout >> Get Specific Files from Local Repo
2. Staging
> git commit  >> Take a `snaphot` to local repository
3. Local Repository
> git push to `Remote Repo` > Send It
> git pull to `Local Repo` > Return It Back
4. Remote Repository

#### Default Branch > `Master` Or `Main`

#### Repo consists of all your commits
#### `Project` is made up of `bunch of commits`
#### Each commit has a `hash code`

#### `HEAD` is a reference of _current branch_

#### Basic Commands
1. status
2. add
3. commit
4. log

- - - - - - -
git log > hist of commits
git status >> Status of repository
git diff
- - - - - - -
### git init
// Link `Server-Repo` with `Local-Repo`
git remote add origin link-of-online-repo Or server-repo
// Get `Clone` Or `Copy` from `Server-Repo`
git clone repo-url
- - - - - - -
### git push
// Push Master Branch
> git push origin master
// Push Specific Branch
> git push origin branch-name
- - - - - - -
### git checkout
git checkout -b 'branch_name'
git checkout created-branch-name
- - - - -- --
### git config
> git config --global user.name 'user-name'
> git config --global user.email 'user-email'
> git config --global --list
- - -- - -- -
### git pull
> git pull > Get all changes from remote repo
> 
- - -- - -- -
### .gitignore
file .gitignore _contains files that must not be uploaded with git files of project
> secret.json
> 
- - -- - -- -
### Branches:
// Url: https://www.youtube.com/watch?v=WtCXZoQqVzI&list=PL_aOZuct6oAogr4UMkWddU7leOXw0QKJS&index=4
> Each branch _includes_ the commits
> Branch _means_ > Make a copy in another place not in main repo 
> When new feature I added successfully successed! Now I can make merge _new feature_ in main repo
> 
### git branch
// Create a new branch
> git branch branch-name
> git branch sample
* Master > Active Branch
// Another way > switch to new branch
> git checkout -b 'new-branch'
sample
// Change Branch
> git checkout created-branch-name
> git branch
// Delete Branch
> git branch -d 'branch-name'
master
* sample > active branch
// All Commits also come to branch
> git log
- --- -------
### git merge
// Merge `New Code` with `Master Code`
// Go to Branch Y want to Update it with New Code
> git checkout branch-to-be-updated
> git checkout master
> git merge branch-of-new-code
> 
- - -- - -- -
# Experiences:
> git commit -am 'Message of Commit'  > Add & Commit at same time
> 
-- ----------- --


