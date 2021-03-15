#### Enable Vim style navigation in Git bash 
`set -o vi` 
#### in order to turn off the vi mode compatibility just run
`set +o vi`
to learn more about flags use `set --help`

## Ok above solution works only for one session, in order to set it permanently 
## you have to modify the `bashrc` or `bash_profile` 


### My vimrc file 
vimrc file path: ~.vim/vimrc \n
this can be reached via `cd ~` take me to the home folder \
`.file` or `.directory` can't be seen by just vi `ls` command \
in order to list all files run `ls -a` \

now go to **.vim** folder and open **vimrc** file \
go to edit mode and edit the file as you wish \
```vim
" Custom Vim configuration 

" mapping NORMAL MODE key 
:imap ii <Esc>

set hlsearch    " highlight all search results
set ignorecase  " do case insensitive search 
set incsearch   " show incremental search results as you type
set number      " display line number
```





