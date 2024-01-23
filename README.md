# differentsheets
Differenr lifehacks and sheets for programming, collected by life experience

# git

## pretty format for logs:

### using
```git log --pretty=format:"%h %ad | %s%d [%an]" --date=short```

### create default config
```
git config --global format.pretty '%h %ad | %s%d [%an]'
git config --global log.date short
```

## main funcs
`git add <./filename/foldername>` - INDEX all/file/folder on changes 

`git commit [--amend] -m "<message>"` - COMMIT all indexed changes with message. If [ammend] - add indexed changes to last commit.

`git tag <tagname>` - ADD TAG as tagname to this commit

`git switch [-c] <hash/tag/HEAD>` - change brain on other with this hash/tag/HEAD. If [-c] - create new branch.

`git checkout <./filename/foldername>` - remove all NO INDEXED changes

`git revert <hash/tag/HEAD>` - CANCEL choosen COMMIT by new commit, but save it in logs

`git reset [--hard] <hash/tag/HEAD> [<./filename/foldername>`] - remove ALL AHEAD COMMIT WITH ALL INDEXES for choosen. If [--hard] - remove all changes, else - no. (THEY WILL LEAVE FROM BRANCH, BUT THEY WILL BE IN REPOSITORY. For full delete - use `git tag -d <tagname>`

`git tag -d <tagname>` - DELETE ALL UNLINKED COMMITS, associated with this tag from repository
