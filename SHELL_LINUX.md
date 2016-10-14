#Linux shell substitues

Must have for newbies or starters with linux commands and terminal, 
zsh or fish will provide much more than standart Bash.

### Numero uno

http://www.zsh.org/

Following installing [OH-MY-ZSH](https://github.com/robbyrussell/oh-my-zsh)


To replace your shell 

```
sudo chsh -s $(which zsh)
```

or if it doesn't work for you - you can try edit directrly 

```sudo nano /etc/passwd ```

file


### Numero dos

http://fishshell.com/

I like fish shell, because i am not a fish in linux command line (and programs, tools, their params). Fish can make it easier to use commands - - smart interactive autocomplete - colors





## What are .bash* files in your ~ dir:

/bin/bash
The bash executable

/etc/profile
The systemwide initialization file, executed for login shells

~/.bash_profile
The personal initialization file, executed for login shells

~/.bashrc
The individual per-interactive-shell startup file

~/.bash_logout
The individual login shell cleanup file, executed when a login shell exits

~/.inputrc
Individual readline initialization file
