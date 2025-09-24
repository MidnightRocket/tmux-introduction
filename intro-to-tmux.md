---
title: "**tmux**"
sub_title: "(A brief introduction to tmux)"
author: "MidnightRocket"
theme:
  name: "catppuccin-frappe"
  override:
    intro_slide:
      title:
        colors:
         foreground: "p:tmux_green"
    palette:
      colors:
        tmux_green: "1ABA1F"
      classes:
        tmux:
          foreground: "p:tmux_green"
---



<!--
  Use the provided presenterm wrapper script to generate the toc.md file
  and launch presenterm.
-->

Table of Contents
 ===
<!-- include: toc.md -->
<!-- end_slide -->


What is <span class="tmux">tmux</span>?
===

> **tmux** is a terminal multiplexer.

<!-- pause -->

- Split windows
- Multiple windows (tabs)
- Keyboard centric
- Works over SSH


<!-- pause -->

```sh +exec +acquire_terminal
./tmux/demo tmux/example-0
```

<!-- end_slide -->
<span class="tmux">tmux</span> basics
===
- Sessions
- Windows
- Panes

<!-- pause -->
```sh +exec +acquire_terminal
./tmux/demo tmux/example-1
```

<!-- 
speaker_note: |
  split
  split -h
  show pane numbers
  new window

  : new
  tmux ls

  session are like workspaces. 
-->

<!-- end_slide -->


<span class="tmux">tmux</span> navigation
===
> tmux is keyboard centric.
> Everything can be done using just the keyboard!


> Keyboard shortcuts work differently from GUI apps
<!-- pause -->


- Prefix key (C-b)
- Commands are given as sequences

<!-- pause -->
```sh +exec +acquire_terminal
./tmux/demo tmux/example-2
```

<!-- end_slide -->


Persistence
===
> tmux is driven by a client-server architecture

<!-- pause -->

- Useful for SSH
- Session survive even if terminal emulator crashes
- Even logging out/in

<!-- pause -->
```sh +exec +acquire_terminal
/// clear
/// printf "\033[?25h" # Clear screen and show cursor.
/// PS1_OVERRIDE='%B%(?.%F{green}.%F{red}%?-)%(!.#.>)%b%u%s%f '
/// export PS1_OVERRIDE
$SHELL
```
<!-- 
speaker_note: |
  client-server arch gives persistence.

  tmux ls
  tmux attach
  show internet interrupt
  tmux re-attach

  Work setup persisted.
  Can log in from different devices.
-->
<!-- end_slide -->

More Awsome <span class="tmux">tmux</span>
===
- Synchronized panes

<!-- pause -->
```sh +exec +acquire_terminal
./tmux/demo tmux/example-3
```

<!-- end_slide -->


Resources
===

- [this presentation](https://github.com/MidnightRocket/tmux-introduction)
- [my-tmux-conf](https://github.com/MidnightRocket/my-tmux-conf)
- [awesome-tmux](https://github.com/rothgar/awesome-tmux)
- [tmate](https://github.com/tmate-io/tmate)
