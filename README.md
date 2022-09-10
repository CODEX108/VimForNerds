# Vim
<img alt= exit_vim height=350px  src="https://pics.onsizzle.com/wq-killal-vim-9-here-are-multiple-ways-to-exit-21791909.png" /> 
Vim a text editor for writing code where you navigate around the screen
with a keyboard instead of a mouse it's based on the original unix text editor
vi which came about in 1976 then, vi improved or vim followed it in 1991 with
a bunch of improvements

Vim is rock stable and is continuously being developed to become even better. Among its features are:
- persistent, multi-level undo tree
- extensive plugin system
- support for hundreds of programming languages and file formats
- powerful search and replace
- integrates with many tools

##  Three modes of Vim
-  insert (i)
-  visual (v)
- command (:)

Command mode (Where you give commands to the editor to get things done . Press ESC for command mode)
Most of them below are in command mode:
```js
x - to delete the unwanted character
u - to undo the last the command and U to undo the whole line
CTRL-R to redo
A - to append text at the end
:wq - to save and exit
:q! - to trash all changes
dw - move the cursor to the beginning of the word to delete that word
2w - to move the cursor two words forward.
3e - to move the cursor to the end of the third word forward.
0 (zero) to move to the start of the line.
d2w - which deletes 2 words .. number can be changed for deleting the number of consecutive words like d3w
dd to delete the line and 2dd to delete to line .number can be changed for deleting the number of consecutive words
```

## Setting up Vim Configuration File
If you have like 20 settings, you  don't want to set them all the time every time you open Vim. So you want to have a settings file a  configuration file that does it for you. And for that you have the **VIM rc file**, which is located  at the user directory
``` vi ~/.vimrc ```

If the file is there, vim loads it, or VIM is going to open it. If it's not there,it will get created  in VIM and Vim is still going to load it. So we're going to open up the VIM rc file .Enter the insert mode and set the reqired settings and customize accordingly

#### *This is just an example*
```js
set number
set relativenumber
set tabstop=3
set autoindent
set shiftwidth=4
set mouse=a
colorscheme slate
```

## Documentation

[Official Vim Documentation](https://www.vim.org/)





