# NVchad

# Vim Commands and Tips

## Basic Operations (Command-line Mode)
*   `:q` - Quit
*   `:w` - Save
*   `:wq` or `:x` - Save and quit
*   `:q!` - Quit without saving (discard changes)
*   `:e <file>` - Edit/open a new file

## Modes
*   `i` - Insert mode (insert text before cursor)
*   `a` - Append mode (insert text after cursor)
*   `o` - Open new line below and enter insert mode
*   `Esc` - Return to Normal mode from any other mode
*   `v` - Visual mode (character-wise selection)
*   `V` - Visual Line mode (line-wise selection)
*   `Ctrl+v` - Visual Block mode (rectangular selection)
*   `:` - Command-line mode (for executing commands)

## Navigation (Normal Mode)

### Character/Line Movement
*   `h` - Move left
*   `j` - Move down
*   `k` - Move up
*   `l` - Move right
*   `0` - Move to the start of the line
*   `^` - Move to the first non-blank character of the line
*   `$` - Move to the end of the line

### Word Movement
*   `w` - Move to the beginning of the next word
*   `e` - Move to the end of the current word
*   `b` - Move to the beginning of the current word

### File Jumps
*   `gg` - Go to the top of the file
*   `G` - Go to the bottom of the file
*   `:<line_number>` or `<line_number>G` - Go to a specific line number
*   `%` - Jump to the matching parenthesis, bracket, or brace

### Screen Movement
*   `H` - Move to the top of the screen
*   `M` - Move to the middle of the screen
*   `L` - Move to the bottom of the screen
*   `zz` - Center the screen on the cursor

## Editing (Normal Mode)

### Copy, Cut, and Paste
*   `yy` - Yank (copy) the current line
*   `yw` - Yank (copy) the current word
*   `p` - Paste after the cursor (or after the current line if a line was yanked)
*   `P` - Paste before the cursor (or before the current line if a line was yanked)
*   `x` - Delete character under cursor
*   `dw` - Delete word
*   `dd` - Delete line

## Search and Replace (Command-line Mode)
*   `/pattern` - Search forward for `pattern`
*   `?pattern` - Search backward for `pattern`
*   `n` - Repeat the last search in the same direction
*   `N` - Repeat the last search in the opposite direction
*   `:s/old/new/g` - Replace all occurrences of `old` with `new` on the current line
*   `:%s/old/new/g` - Replace all occurrences of `old` with `new` throughout the entire file
*   `:%s/old/new/gc` - Replace all occurrences of `old` with `new` throughout the entire file, with confirmation for each replacement

## Window and Tab Management
*   `:split` - Create a horizontal split window
*   `:vsplit` - Create a vertical split window
*   `Ctrl+w w` - Switch between windows
*   `Ctrl+w h/j/k/l` - Move to the window left/down/up/right
*   `Ctrl+w +` - Increase current window height
*   `Ctrl+w -` - Decrease current window height
*   `Ctrl+w >` - Increase current window width
*   `Ctrl+w <` - Decrease current window width
*   `:tabnew` - Create a new tab
*   `gt` - Go to the next tab
*   `gT` - Go to the previous tab
*   `:Ex` or `:Vex` - Open Netrw (Vim's file explorer) in a horizontal or vertical split, respectively
