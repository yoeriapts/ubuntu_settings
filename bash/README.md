# Bash settings

How to use these 'bash' settings:

Clone this repo using git/ssh to ~/ubuntu_settings (default location):
```bash
$ git clone git@github.com:yoeriapts/ubuntu_settings.git
```

To use the `bash_aliases`, create a symlink:

```bash
$ cd ~
$ ln -s ~/ubuntu_settings/bash/bash_aliases .bash_aliases
```
and add the following to `.bashrc` (Note: it may already be in there!)
```bash
# bash_aliases
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi
```

If you want to use the history manipulation defined in `bash_extras`, create a symlink:
```bash
$ cd ~
$ ln -s ~/ubuntu_settings/bash/bash_extras .bash_extras
```
and add the following to `.bashrc` 
```bash
# bash_aliases
if [ -f ~/.bash_extras ]; then
    . ~/.bash_extras
fi
```
To use the 'z' (jump around) utility;

First clone the 'z - jump around' repo:
```bash
$ mkdir ~/workspace
$ git clone https://github.com/rupa/z.git ~/workspace/z
```

then add the following to .bashrc (check location of z!)

```bash
# z - jump around
if [ -f ~/workspace/z/z.sh ]; then
    . ~/workspace/z/z.sh
fi
```

If you want to use gitprompt:
```shell
$ ln -s ~/ubuntu_settings/bash/gitprompt .gitprompt
```
If you want to use some special key-bindings:
```shell
$ ln -s ~/ubuntu_settings/bash/inputrc .inputrc
```
and add the following to .bashrc
```bash
# Git prompt
if [ -f ~/.gitprompt ]; then
    . ~/.gitprompt
fi
```

To manipulate some 'keystrokes' on the command line:

```bash
bind -P

ctrl-w: unix-word-rubout: kill word backward
ctrl-r: reverse-search-history
ctrl-x ctrl-e: edit-and-execute-command: use $EDITOR to edit current line
ctrl-f: reverse-search-history after you started typing :-)
ctrl-e: end-of-line: go to eol and start editing
```

## Use with zsh (Z-shell)

### Use with vanilla zsh

For the moment, from all the things mentioned above, only the bash_aliases file can be used with zsh:

symlink the bash aliases file (will be read when processing the ~/.zshrc file)
```bash
$ ln -s ~/ubuntu_settings/bash/bash_aliases ~/.zsh/rc/aliases
```

### Use with oh-my-zsh

users are encouraged to define aliases within the ZSH_CUSTOM folder. So, create a link:
```bash
$ ln -s ~/ubuntu_settings/bash/bash_aliases $ZSH_CUSTOM/aliases.zsh
```

--Yoeri
