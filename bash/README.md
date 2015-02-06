Bash settings
===============

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


--Yoeri
