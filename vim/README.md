Vim settings
=============

```bash

$ cd ~
$ ln ubuntu_settings/vim/vimrc .vimrc
$ ln -s ubuntu_settings/vim/vim .vim

$ ll -d .vim*
lrwxrwxrwx 1 yoeri yoeri    23 Oct 21 22:12 .vim -> ubuntu_settings/vim/vim/
-rw------- 1 yoeri yoeri 17822 Oct 21 22:11 .viminfo
-rw-rw-r-- 2 yoeri yoeri 10885 Oct 12 21:33 .vimrc

$ vim # start vim to interactively download 
      #  all the vim-addons referred to in the vimrc file
      
```

