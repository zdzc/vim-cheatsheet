# vim-cheatsheet

## Command
- `:help <term>` - open Vim's help
- `:e <path>` - edit a file
- `:w` - save the current file
- `:q` - quit the current window
- `:x` - equivalent to `:wq`

## Cursor Movement
### Basic
- `h` - left
- `j` - down
- `k` - up
- `l` - right
- `0` - the start of the line
- `$` - the end of the line
- `f<char>` - next occurence of `<char>` on current line
- `F<char>` - previous occurence of `<char>` on current line
- `t<char>` - left of `f<char>`
- `T<char>` - left of `F<char>`
- `G` - the last line
- `_G` - nth-line
- `^f` - move forward a page
- `^b` - move backward a page
### Word
- `w` - move forwards to the start of a word
- `W` - move forwards to the start of a WORD
- `e` - move forwards to the end of a word
- `E` - move forwards to the end of a WORD
- `b` - move backwards to the start of a word
- `B` - move backwards to the start of a WORD
### Other
- `%` - matching bracket
- `{` - next paragraph
- `}` - previous paragraph

## Editing
- `i` - insert before the cursor
- `I` - insert before first non-blank
- `a` - insert after current character
- `A` - insert at the end of the line
- `o` - insert new line below the cursor and insert text
- `O` - insert new line above the cursor and insert text
- `x` - delete character under the cursor
- `d<motion>` - delete the text for `<motion>`
- `dd` - delete a line
- `D` - delete until the end of the line
- `c<motion>` - change the text for `<motion>`
- `cc` - change the entire line
- `C` - change the text until the end of the line

## Visual Mode
- `v` - enter visual mode
- `Shift+v` - enter visual mode linewise
- `Ctrl+v` - enter visual mode blockwise

## Searching
- `/pattern` - search forward for pattern
- `?pattern` - search backward for pattern
- `n` - repeat the search in same direction
- `N` - repeat the search in opposite direction
- `:noh` - remove search highlighting

## Configuration
- `set clipboard+=unnamedplus` - integrate system clipboard to vim
- `set expandtab` - automatically replaces tab to spaces on insert mode

## Glossary
- `word` - A word consists of a sequence of letters, digits and underscores, or a sequence of other non-blank characters, separated with white space (spaces, tabs, <EOL>). This can be changed with the 'iskeyword' option.  An empty line is also considered to be a word.
- `WORD` - A WORD consists of a sequence of non-blank characters, separated with white space.  An empty line is also considered to be a WORD.
