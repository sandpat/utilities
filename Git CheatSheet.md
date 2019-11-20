# Git CheatSheet
### Branch Deletion
* Local Branch

	```sh
	git branch -d branch_name
	```
	or
	
	```sh
	git branch -D branch_name
	```
	
	where `-d` stands for `--delete` while `-D` means `--delete --force`
	
* Remote Branch

	```sh
	git push <remote_name> --delete <branch_name>
	```
	or
	
	```sh
	git push <remote_name> :<branch_name>
	```
	
	If we want to push a local branch to remote deleting the local copy, we can do 
	
	```sh
	$ git push -d <remote_name> <branch_name>
	```
	or
	 
	```sh
	git push --delete <remote_name> <branch_name>
	```

### Clone a specific branch directly
```sh
$ git clone --single-branch --branch <branch> <repo-ref>
```

### Create a new branch from specific commit
```sh
$ git checkout -b <branch> <sha1-of-commit>
```

### Print trace of `git clone` call
```sh
$ env GIT_TRACE_CURL=true git clone <repo-ref>
```

### Check Remote urls
```sh
$ git remote --verbose
```
or

```sh
$ git remote -v
```
will give the `fetch` and `push` remote urls.

### List all tags
```
$ git tag
```

### List last tag
```
$ git describe --tags --abbrev=0
```

### List tags for a remote repository
```
$ git ls-remote --tags <repo-ref>
```
