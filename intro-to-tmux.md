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

<!-- include: toc.md -->



What is <span class="tmux">tmux</span>?
===

> **tmux** is a terminal multiplexer.

<!-- pause -->

- Split windows into multiple panes
- Multiple windows
- Keyboard centric
- Works over SSH


<!-- pause -->

```sh +exec +acquire_terminal
./tmux/demo tmux/example-0
```

<!-- end_slide -->
Demo
===

```sh +exec +acquire_terminal
./tmux/demo
```


<!-- end_slide -->

Resources
===

- [github.com/rothgar/awesome-tmux](https://github.com/rothgar/awesome-tmux)
- 
