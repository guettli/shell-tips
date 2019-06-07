# i-like-the-command-line
I like the command line: My favorite tips and tricks

List all Python processes of the corrent user
pgrep -au $USER -f python

Kill them. Same as above, but without "-a" since you don't want to list the full command line
pgrep -au $USER -f python


cool prompt.


https://stackoverflow.com/questions/56494149/bash-alternative-zu-ctrl-r


reset at the front: if there is a lot of output, and you want to start to look at the examples from top to bottom:

you@host:~/> reset; find */* -name '*.py'| grep -P ... | xargs grep FooBar

of course this would work, too:

you@host:~/> find */* -name '*.py'| grep -P ... | xargs grep FooBar | less


Pager "less" ... then "-S" chop long lines
