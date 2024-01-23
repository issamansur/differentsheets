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
