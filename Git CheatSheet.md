# Git CheatSheet
### Branch Deletion
* Local Branch

	`git branch -d branch_name`
	<br>or<br>`git branch -D branch_name`
	
	where `-d` stands for `--delete` while `-D` means `--delete --force`
	
* Remote Branch

	`git push <remote_name> --delete <branch_name>`
	<br>or<br> 
	`git push <remote_name> :<branch_name>`
	
	If we want to push a local branch to remote deleting the local copy, we can do `git push -d <remote_name> <branch_name>` or `git push --delete <remote_name> <branch_name>`

### Clone a specific branch directly
`$ git clone --single-branch --branch <branch> <repo-ref>`
### Print trace of `git clone` call
`$ env GIT_TRACE_CURL=true git clone <repo-ref>`
### Check Remote urls
`$ git remote --verbose`
or
`$ git remote -v`
will give the `fetch` and `push` remote urls.