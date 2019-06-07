# i-like-the-command-line
I like the command line: My favorite tips and tricks

List all Python processes of the corrent user
pgrep -au $USER -f python

Kill them. Same as above, but without "-a" since you don't want to list the full command line
pgrep -au $USER -f python
