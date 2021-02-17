# Git-bash for Windows

1. Download and install Git-bash from https://gitforwindows.org/
2. Download and install Con-Emu (Optional)

3. Clone this repo


Clone this repo to ~/ubuntu_settings (default location):
```bash
$ cd ~
$ git clone https://github.com/yoeriapts/ubuntu_settings.git
```

Clone the 'z - jump around' repo
```bash
$ mkdir ~/git_workspace
$ git clone https://github.com/rupa/z.git ~/git_workspace/z
```

When freshly installed, git-bash only has a `.bash_history` file
```bash
$ ll .bash*
-rw-r--r-- 1 yoeri 197610 239 jul 30 15:07 .bash_history
```

link to files from ~/ubuntu_settings/git_bash
```bash
$ ln ~/ubuntu_settings/git_bash/bash_profile .bash_profile
$ ln ~/ubuntu_settings/git_bash/bashrc .bashrc
```
link to aliases from ~/ubuntu_settings/bash
```bash
$ ln ~/ubuntu_settings/bash/bash_aliases .bash_aliases
```

Start a new git-bash session to activate the new settings

copy the ~/ubuntu_settings/git_bash/bin/* to ~/bin 
note that ~/bin is already in your $PATH


