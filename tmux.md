# Tmux

## Sessions

```
# Switch to another session
<C-b> + s
# select the session

# Switch to last used session
<C-b> + L
```

## Mouse mode with Cygwin in windows

```
set mouse on|off
```

### Use terminal copy/paste mode

Press SHIFT and select a zone/mouse middle click.

### Copy selection to system clipboard

```
bind-key -T copy-mode MouseDragEnd1Pane send-keys -X copy-selection \; save-buffer /dev/clipboard
```

### Paste selection from system clipboard with middle click

```
bind-key -T root MouseDown2Pane load-buffer /dev/clipboard \; paste-buffer
```

## Jump to a window

```
prefix-key <window-index>
prefix-key ' <window-index>
prefix-key w
```

## Move a pane in its window

Move the current pane to the destination pane, splitting it vertically by
default.

```
move-pane -t <dst-pane>

# Split horizontally the destination pane.
move-pane -t <dst-pane> -h
```

## Swap panes

prefix-key {
prefix-key }

```
swap-pan [-UD]
```

## Sync commands

```
setw synchronize-panes on|off
```

## Resize panes equaly

```
select-layout even-vertical
select-layout even-horizontal
```
