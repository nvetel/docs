# Docs

## Git

### Move a branch (change the branch pointer target)

```
git branch -f <commit>
```

### Pull "force" (reset local branch to a remote branch)

```
# Reset to a remote branch
git reset --hard <remote-branch>

# Reset to the upstream branch
git reset --hard @{upstream}
```

### Show file at a specific commit

```
git show REVISION:PATH
```

## Less

```
# don't wrap long lines
less --chop-long-lines/-S
```

## Sed

```
# Filter logs from date to date
sed -n '/2018-04-12 14:44:00.000/,/2018-04-12 14:45:00.000/p' log_file
```
