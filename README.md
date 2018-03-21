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

## Tmux

### Mouse mode with Cygwin in windows

#### Use terminal copy/paste mode

Press SHIFT and select a zone/mouse middle click.

#### Copy selection to system clipboard

```
bind-key -T copy-mode MouseDragEnd1Pane send-keys -X copy-selection \; save-buffer /dev/clipboard
```

#### Paste selection from system clipboard with middle click

```
bind-key -T root MouseDown2Pane load-buffer /dev/clipboard \; paste-buffer
```
