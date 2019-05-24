# Git CheatSheet
### Clone Branch Directly
`$ git clone --single-branch --branch <branch> <repo-ref>`
### Print trace of `git clone` call
`$ env GIT_TRACE_CURL=true git clone <repo-ref>`
### Check Remote urls
`$ git remote --verbose`

will give the `fetch` and `push` remote urls.