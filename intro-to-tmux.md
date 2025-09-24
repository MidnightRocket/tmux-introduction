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


<!-- end_slide -->


<span class="tmux">tmux</span> navigation
===
> tmux is keyboard centric.
> Everything can be done using just the keyboard!

<!-- pause -->

- Prefix key (C-b)
- Commands are given as sequences

<!-- pause -->
```sh +exec +acquire_terminal
./tmux/demo tmux/example-3
```

<!-- end_slide -->


Persistence
===
> tmux is driven by client server architecture

<!-- pause -->

- Useful for SSH
- Session survive even if terminal emulator crashes
- Even loggin out/in

<!-- pause -->
```sh +exec +acquire_terminal
/// clear
/// printf "\033[?25h" # Clear screen and show cursor.
/// PS1_OVERRIDE='%B%(?.%F{green}.%F{red}%?-)%(!.#.>)%b%u%s%f '
/// export PS1_OVERRIDE
$SHELL
```

<!-- end_slide -->


Resources
===

- [awesome-tmux](https://github.com/rothgar/awesome-tmux)
