# git-cli

[Course](https://www.youtube.com/watch?v=Q5Eb3jBvFEE&list=PL_aOZuct6oAogr4UMkWddU7leOXw0QKJS)

### Architectur of Git

#### Work Area

add files of working area to stage area
`git add file_name.type`

get specific files from local repo
`git checkout`

#### Stage Area

take a snaphot to local repo
`git commit`

#### Local Repo


`git push`
`git pull`

#### Remote Repo

---

### Notes


- Each _repo_ has a _default branch_ `Master`

- _Repo_ consists of the `commits`
- Project is made up of _bunch of commits_

- Each commit has a `hash code`
- _HEAD_ is a reference of _current branch_

---

### git config

Developer name
`git config --global user.name 'user-name'`
Developer email
`git config --global user.email 'user-email'`

`git config --global --list`

- - -
### git init

`git init`

add a remote repo with [url] and an alias of [name]
`git remote add [name][url]`

get clone || copy from server repo
`git clone repo_url`

merge main in master
`git branch -M main`

- - -
### git push

push changes to a remote repo called [name] to branch [b]
`git push [name][b]`

- - -
### git pull

Pull the changes from the repos
`git pull [name][b]`
Pull any changes from a remote repo called [name] from branch [b]

<!-- ###### _before make `pull req` you should commit your changes_ -->

- - -
### `.gitignore` File

.gitignore file includes the files that must not be uploaded with staged files of project
name*of_file.type example \_secret.json*

---

### About Branches

[About branches](https://www.youtube.com/watch?v=WtCXZoQqVzI&list=PL_aOZuct6oAogr4UMkWddU7leOXw0QKJS&index=4)
Each branch consists of _commits_
`What Branch?` makes a copy of the _current branch_ in _another place_ you can modify as you wish without affecting the origin

###### _So when new feature I added successfully done, Now I can make merge new feature in main repo by merge the branches with each other_

### git branch

_Create_ a new branch
`git branch _new_branch_name_`

_Create_ new branch & switch to new branch
`git checkout -b _new_branch_name`

_Change_ Branch
`git checkout _created_branch_name_`

_Delete_ Branch
`git branch -d 'branch-name'`

Show _all branches_ of current repo
`git branch`

---

### git merge

[Merge](https://www.youtube.com/watch?v=74ZuPrgzRpE)
merge new code from _specific branch_ with _master_

switch into master
`git checkout _master_`

merge branch with master
`git merge _branch-to-merge_`

لابد وان يكون هناك فروع أٌخري غير الافتراضي بحيث يكون كل فرع مختص بجزء معين من المشروع
والأساسي يُستخدم لرفع المشروع

---
### git diff

view occured differences of files
`git diff file.type` `git diff`

---

### git restore

return to latest state before make changes in working tree

- _before stage_ `git restore file.type` `git restore`

- _after stage_ `git restore --staged file.type`

---

<!--

#### Notes:
git commit -am 'Message of Commit'

--- -->

### Commands

`git status` `git add` `git commit` `git log` `git diff`

---

### About Contributors Or Collaborators

1. Settings
1. Collaborators
1. Add people Button
1. Type & Add users names

---

### GITHUB Use Cases! & GIT Solutions

#### Start a new project

- git init
- git clone remote-repo-url

#### Upload new updates with main branch

- git commit -m ‘message of commit’
- git push origin master

#### Download from remote repo on master branch

- git pull origin master

#### Changes are not correct in working tree, the need to discard changes & return to lastest state that means _before stage_!

  <!-- _Minus means something deleted, Plus means something added_ -->

<!-- - git diff file.type -->

- git restore file.type

#### Changes are not correct in stage area, the need to discard changes & return to lastest state!

<!-- - git diff file.type -->

- git restore –-staged file.type

#### The need to return latest state before commit

[geeksforgeeks](https://www.geeksforgeeks.org/how-to-undo-a-commit-in-git/)

`git --help`

reset: reset current HEAD to the specified state

- git log --pretty=one

  soft is used if you want to keep your changes

- git reset –-soft HEAD^

  hard is used if you don’t want to keep your changes

- git reset –-hard HEAD^



