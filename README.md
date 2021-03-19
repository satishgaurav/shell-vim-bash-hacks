
## Enable Vim style navigation in Git bash 
`set -o vi` 
##### in order to turn off the vi mode compatibility just run
`set +o vi`
to learn more about flags use `set --help`

#### Ok above solution works only for one session, in order to set it permanently 
#### you have to modify the `bashrc` or `bash_profile` 


### My vimrc file 
vimrc file path: ~.vim/vimrc  <br /> 
this can be reached via `cd ~` take me to the home folder \
`.file` or `.directory` can't be seen by just vi `ls` command \
in order to list all files run `ls -a`  

now go to **.vim** folder and open **vimrc** file \
go to edit mode and edit the file as you wish  
```vim
" Custom Vim configuration 

" mapping NORMAL MODE key 
:imap ii <Esc>

set hlsearch    " highlight all search results
set ignorecase  " do case insensitive search 
set incsearch   " show incremental search results as you type
set number      " display line number
```

### My .bash_profile file 
I have also enabled the vim mode in bash shell. 
Now the the key binding does work by default by just setting up vi mode \
by the way you can vi mode using `set -o vi` and disable it using command `set +o vi` 

However the above solution only works for one session in order to bring the change to all the session \
you have modify `.bashrc` or `.bash_profile` file present on the home directory. you can reach home \ 
using the command `cd ~` now list all files using command `ls -a` 

```bash
## this will keep the vim mode enabled in git bash 
## to turn-off mode change "-" to "+".
set -o vi
bind '"ii":vi-movement-mode'
```

Now I have done it only the basic modification. If you want to modify extra things <br/>
then these linkes can be useful 
1. https://unix.stackexchange.com/questions/303282/in-bash-vi-mode-map-jk-to-exit-insert-mode
2. https://stackoverflow.com/questions/6839006/map-jj-to-esc-in-inputrc-readline






