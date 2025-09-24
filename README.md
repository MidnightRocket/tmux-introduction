# tmux introduction
This presentation and demo of [tmux](https://github.com/tmux/tmux/wiki), is made with
[presenterm](https://github.com/mfontanini/presenterm) and a collection of shell scripts. 

# Running the presentation
Make sure to have [presenterm installed](https://mfontanini.github.io/presenterm/install.html).

A wrapper script is included in this repo which autogenerates a Table of Contents. 

To present use the wrapper script:
```sh
./presenterm intro-to-tmux.md
```
This works on most Linux and Mac OSes. 

To allow for code execution which is required to run the demos use:
```sh
./presenterm -x intro-to-tmux.md
```

# Demos
These demos are self contained and isolated from any default tmux server & sessions running on the host. 
To run them, at least tmux most be installed. 
