
## Enable Vim style navigation in Git bash 
`set -o vi` 
##### to turn off the vi mode compatibility just run
`set +o vi`
to learn more about flags use `set --help`

Did you like the above taste? if yes, then you might want to do it for every session. The above solution works only for single session, 
In order to set it permanently we have to modify the `bashrc` or `.bash_profile`. It is present on the home directory to go there just run `cd ~`. In order to see the `.file_name` or `.directory_name` just run `ls -a`.  

Pasting above code will enable the vim mode for all session. I have also enabled the vim mode in bash shell. Now I wanted to map few shorcuts. Like using **`ii`** to go from edit mode to normal mode instead of **`ESC`** key. It doesn't work by default. To do that just edit the file with the following command. Well you can do all sorts of mapping according to your convenience. 

### My .bash_profile file 

```bash
## this will keep the vim mode enabled in git bash 
## to turn-off mode change "-" to "+".
set -o vi
bind '"ii":vi-movement-mode'
```

### How to modify vimrc file?
If you learning or using vim then you might want to edit you vimrc file. In order to modify the vimrc file first you have to locate it. Generally it is present on the home folder. Depending on the operating system this can be different. I am uisng Windows OS with WSL (Window Sub-system for Linux). My vimrc was not present on the home folder. So I created the .vim folder and then vimrc file. In order to create this you have to navigate to you home directory using command `cd ~`. Once you are there you won't see file and folder names with **.** in front of it (like `.file_name` or `.directory_name`) with simple `ls` command. You have to run `ls -a`. Now you would be able to see all the files. 

Now go to **.vim** folder and open **vimrc** file using **vim vimrc** if the file does not exist then this command will create however keep in mind that after you are done editing you save using command `:wq`. Or you can just use plain text editor to achieve the same task as you wish. 

### My vimrc file 
```vim
" Custom Vim configuration 

" mapping NORMAL MODE key 
:imap ii <Esc>

set hlsearch    " highlight all search results
set ignorecase  " do case insensitive search 
set incsearch   " show incremental search results as you type
set number      " display line number
```

Now I have done it only the basic modification. If you want to modify extra things <br/>
then these linkes can be useful 
1. https://unix.stackexchange.com/questions/303282/in-bash-vi-mode-map-jk-to-exit-insert-mode
2. https://stackoverflow.com/questions/6839006/map-jj-to-esc-in-inputrc-readline

