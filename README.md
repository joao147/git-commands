# Basic Git Commands

## Help
### git
Shows help.

### git <_git command_> -h
Shows help from specified command. ex: git commit -h.

## Init
### git init
It's used to start a git in repository that was run.

### git init DirectoryName
It's used to start a git repository in a directory. Can be a new directory or already exist.

### git init < path >
It's used to start a git repository in a directory in last item of path.

## Add
### git add FileName
This command is used to add an specific file to your stage.

### git add .|*|--all
Adds all modified files to stage.

### git add -u|--update
Adds all modified files to stage, unless untracked files.

## Status
### git status
Shows all modifications in your git directory.

## Restore
### git restore FileName
Restore the file as it was.

### git restore FileName --staged
Restore the file that was stagged as it was.

## Diff
### git diff
Print all difference on files, it's compare current state with last commit.

### git diff <_hash commit_>
Print all difference in files that compare current state with hash commit.

### git diff <_hash commit_> <_other hash commit_>
show you all difference in files comparing both commits hash.

## Commit
### git commit
Use to track/commit modifies that was added/staged by add command.

### git commit -m "Something"
Message is write in command, different as above command that vi is open automatically.

### git commit -a
Same of git commit, but commit unstaged files too. It's like you use "git add .", after "git commit".

### git commit -am "Something"
It's a combination of both above, It's the seem you run "git add .", after "git commit -m "Something"".

### git commit --amend
It's used to change your last commit, you can change message or some modification in files that you added.

## Logs
### git log
Shows all commits, with some details.

### git log --oneline
Shows all commits, with only commit hash and message.

### git log -<_number_>
Shows last _N_ commits, details as git log.

### git log --graph --decorate
Print commits log with a better UI, you can see it better when you're working more than one branch.

#### Observation about _git log_
You can combine option to improve visibility.

## Tag
### git tag
Shows you all tags that have been created.

### git tag TagName
It's create a tag in your current HEAD.

### git tag -a TagName
Same as last command, but you add a comment/description to new tag.

### git tag TagName <_hash commit_>
It's create a tag in commit which is represent by _hash commit_. You can use "-a" to add comment/description too.
