Sammy tmux config

Installation
------------

  Download:

```bash
brew update
brew install tmux

git clone https://github.com/SammyLin/tmux-config.git ~/.tmux

# Copy tmux plugin Manager
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# Copy tmux config to home:
ln -s ~/.tmux/.tmux.conf ~/.tmux.conf

tmux

tmux source ~/.tmux.conf


```

Then `Control + a ` then `I`

Install Plugin

Plugin
-----

- tmux-plugins/tpm
- tmux-plugins/tmux-sensible
- tmux-plugins/tmux-prefix-highlight
- tmux-plugins/tmux-resurrect
- tmux-plugins/tmux-open
- tmux-plugins/tmux-yank
- tmux-plugins/tmux-battery
- erikw/tmux-powerline

You can install any Plugin in `~/.tmux.conf`

  Example:

```
set -g @plugin 'erikw/tmux-powerline'
```

Then `Control + a ` then `I`

  Launch tmux:
```
tmux
```
  And press `Control + a` then `d` to go back to the terminal.

  Update config:

```bash
tmux source-file ~/.tmux.conf
```

Start tmux
----------

To start a session:

`tmux`

To reattach a previous session:

`tmux attach`

To reload config file

`<Control + b>:` (which could Ctrl-B or Ctrl-A if you overidden it) then `source-file ~/.tmux.conf`

Commands
--------

Our prefix/leader key is `Control + a` now (just like the `screen` multiplexer). This sequence must be typed before any tmux shortcut.

* `Control + a` before any command
* `Control + a` then `?` to bring up list of keyboard shortcuts
* `Control + a` then `"` to split window
* `Control + a` then `<Space>` to change pane arrangement
* `Control + a` then `o` to rotate panes
* `Control + a` then `h`, `j`, `k`, `l` to move left, down, up, right. Respectively. (vim hjkl)
* `Control + a` then `;` to go to last panel

Beyond your first window:

* `Control + a` then `c` to create a new window
* `Control + a` then `n` to next window
* `Control + a` then `p` to previous window
* `Control + a` then `[0-9]` move to window number
* `Control + a` then `&` to kill window

Custom:

* `Control + a` then `m` to switch to ``main-horizontal`` layout with the main window at 60% height.

Fork From
----

* Github: http://www.github.com/tony
* Website: http://www.git-pull.com
* LICENSE: MIT
* Author: Tony Narlock (tony@git-pull.com)
