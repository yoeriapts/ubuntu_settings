Bash settings
===============

How to use these 'bash' settings:

Clone this repo to ~/ubuntu_settings (default location):
```bash
$ git clone https://github.com/yoeriapts/ubuntu_settings.git
```

Create some symlinks
```bash
$ cd ~
$ ln -s ~/ubuntu_settings/bash/bash_aliases .bash_aliases
$ ln -s ~/ubuntu_settings/bash/gitprompt .gitprompt
$ ln -s ~/ubuntu_settings/bash/inputrc .inputrc
```

add the following to .bashrc
```
# Git prompt
if [ -f ~/.gitprompt ]; then
    . ~/.gitprompt
fi
```

keystrokes on the command line:

```
bind -P

ctrl-w: unix-word-rubout: kill word backward
ctrl-r: reverse-search-history
ctrl-x ctrl-e: edit-and-execute-command: use $EDITOR to edit current line
ctrl-f: reverse-search-history after you started typing :-)
ctrl-e: end-of-line: go to eol and start editing
```

Use with zsh (Z-shell)

symlink the bash aliases file (will be read when processing the ~/.zshrc file)
```
$ ln -s ~/ubuntu_settings/bash/bash_aliases ~/.zsh/rc/aliases
```

--Yoeri
