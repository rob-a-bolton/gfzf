# What is gfzf?
gfzf is a script which wraps `fzf` with a couple of temp files and a terminal, piping input in/out of the script transparently.  

You may use this as a drop-in replacement for simple dmenu use-cases (i.e. no-opt calls to dmenu, just piping data in/out)  

# Usage
Pipe newline-delimited data into `gfzf` and capture its output.  
If you have `alacritty` or `kitty` installed, one of these shall be picked as the popup terminal (in that order of preference).  
To override this you can supply a terminal command by exporting `GFZF_TERM` to the script. The terminal must allow the `--class` option. If it does not, edit this out the script or just write a wrapper script around your terminal that ignores all arguments.


# Requirements
`fzf`, `bash`  
