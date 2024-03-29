# Vim

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
Sure! Here's an example of explaining "Basic Vim Usage" using Markdown:

## Basic Vim Usage

### Opening a File
To open a file in Vim, you can use the command `vim <filename>` in your terminal. For example, to open a file called "example.txt," you'd use `vim example.txt`.

### Switching to Normal Mode
By default, Vim opens in normal mode. If you are not in normal mode, press the `Esc` key to switch to it.

### Moving the Cursor
In normal mode, you can move the cursor using the arrow keys or these common navigation commands:
- `h`: Move left
- `j`: Move down
- `k`: Move up
- `l`: Move right

### Entering Insert Mode
To start typing or editing text, you need to enter insert mode. Press `i` (for insert) in normal mode to switch to insert mode.

### Saving a File
To save changes to the file, you need to be in normal mode. First, press `Esc` to ensure you are in normal mode, and then use the command `:w` (short for write) and press `Enter`. This will save the file without closing Vim.

### Closing a File
To close the file and exit Vim, ensure you are in normal mode (`Esc`), and then use the command `:q` (short for quit) and press `Enter`. If you have unsaved changes, Vim will prevent you from exiting and prompt you to save the changes first.

### Saving and Quitting in One Command
To save changes and quit Vim in one command, you can use `:wq` and press `Enter`.

### Discarding Changes and Quitting
If you want to quit Vim without saving any changes, you can use `:q!` and press `Enter`. This will forcefully exit Vim without saving.

### Copying and Pasting Text
In normal mode, you can copy text by moving the cursor to the start of the text you want to copy and then pressing `v` to enter visual mode. Move the cursor to select the desired text and press `y` (short for yank) to copy it. To paste the copied text, press `p` in normal mode.

### Undo and Redo
In normal mode, you can undo changes with the `u` command and redo changes with `Ctrl + r`.

Remember to use proper Markdown formatting and headings to make your content organized and easy to read. Markdown supports basic formatting such as bold, italic, code blocks, bullet points, and more, which you can utilize to enhance the presentation of your explanations.

Certainly! Below is a Markdown-based Vim tutorial for intermediate and advanced users. Feel free to modify and expand as needed:

## Intermediate
1. [**Advanced Movement**](#advanced-movement)
2. [**Working with Multiple Files**](#working-with-multiple-files)
3. [**Customizing Vim**](#customizing-vim)
4. [**Advanced Editing**](#advanced-editing)
5. [**Advanced Search and Replace**](#advanced-search-and-replace)
6. [**Working with Macros**](#working-with-macros)

## Advanced Movement

### 1. Marks

Use marks to quickly navigate between different parts of a file.

- Set a mark: `m{letter}`
- Jump to a mark: \`{letter}

### 2. Jumps and Change List

Navigate through jump locations and track changes.

- Jump to the previous location: `Ctrl+O`
- Jump to the next location: `Ctrl+I`
- View change list: `:changes`

## Working with Multiple Files

### 1. Buffers

Manage multiple files using buffers.

- Open a file in a new buffer: `:badd {file}`
- Switch between buffers: `:bnext`, `:bprev`
- List all buffers: `:ls`

### 2. Tabs

Organize buffers using tabs.

- Open a new tab page: `:tabnew`
- Switch between tabs: `gt` (next tab), `gT` (previous tab)
- Close a tab: `:tabclose`

## Customizing Vim

### 1. Configuration Files

Personalize your Vim environment by editing your `vimrc` file.

- Edit vimrc: `:e $MYVIMRC`
- Reload vimrc: `:source $MYVIMRC`

### 2. Plugins

Extend Vim's functionality with plugins.

- Use a plugin manager like [Vim-Plug](https://github.com/junegunn/vim-plug).
- Install plugins: Add `Plug 'user/repository'` to your vimrc, then run `:PlugInstall`.

## Advanced Editing

### 1. Visual Mode

Perform advanced text manipulation in visual mode.

- Visual block mode: `Ctrl+V`
- Visual line mode: `Shift+V`

### 2. Registers

Utilize registers to copy and paste text.

- Yank to a register: `"ayy`
- Paste from a register: `"ap`

## Advanced Search and Replace

### 1. Global Commands

Execute commands on specific lines or patterns.

- Run a command on all lines matching a pattern: `:g/pattern/command`

### 2. Substitution with Confirmation

Perform substitutions with confirmation.

- Substitute all occurrences in a line: `:s/pattern/replacement/gc`

## Working with Macros

### 1. Recording Macros

Automate repetitive tasks using macros.

- Record a macro: `q{register}`
- Execute a macro: `@{register}`

### 2. Repeat Last Macro

Repeat the last recorded macro.

- Repeat last macro: `@@`

---

These are just a few examples of the many advanced features Vim has to offer. Experiment with these concepts and explore the vast world of Vim customization and efficiency. Happy editing!

## Documentation

[Official Vim Documentation](https://www.vim.org/)





