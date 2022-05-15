# Shell Tips


I like the command line since 1996. Here my favorite tips and tricks. 

I use the shell Bash on Linux. But most of these tips will work on Mac, too.

# Shell only for interactive usage

I like to use the shell interactively. I don't write shell scripts. If some lines should persist, then I use Python code and stored in a git repo.

# pgrep

List all Python processes

```
pgrep -af python
```

```
 -a, --list-full           list PID and full command line
 -f, --full                use full process name to match
```

If you want to terminate processes use `pkill`.


# reset


If you start a command which has a lot of output, and you want to start to look at the first lines at the top, then `reset` helps you:

```
you@host:~/> reset; command-with-a-lot-of-output
```

This would work too. But often I prefer `reset`

```
you@host:~/> command-with-a-lot-of-output | less
```

# direnv

[direnv](https://direnv.net/) loads and unloads environment variables depending on the current directory.

Just create a `.envrc` file in a directory, and your shell will automatically load the environment variables if you `cd` into this directory.




# Related

* [Python Tips](https://github.com/guettli/python-tips)
* [Django Tips](https://github.com/guettli/django-tips) (Web-Framework)
* [Desktop Tips](https://github.com/guettli/desktop-tips-and-tricks)
* [Git Tips](https://github.com/guettli/git-tips)
* [Guettli Working-out-Loud](https://github.com/guettli/wol)
