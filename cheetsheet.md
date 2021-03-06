___
### GLOBAL

`:q`                  quit Vim. This fails when changes have been made. Use !.

`:help keyword`       open help for keyword

`:saveas file`        save file as

`:close`              close current pane

`K`                   open man page for word under the cursor
___
### CURSOR MOVEMENTS

`h`                   move left

`j`                   move down

`k`                   move up

`l`                   move right

`w`                   jump by start of words (punctuation considered words)

`e`                   jump to end of words (punctuation considered words)

`b`                   jump backward by words (punctuation considered words)

`^`                   first non-blank character of line

`0`                   (zero) start of line

`$`                   end of line

`gg`                  go to first line

`G`                   go to last line

`:n`                  go To line n

`nG`                  go To line n

`)`                   move the cursor forward to the next sentence.

`(`                   move the cursor backward by a sentence.

`{`                   move the cursor a paragraph backwards

`}`                   move the cursor a paragraph forwards

`H`                   move the cursor to the top of the screen.

`M`                   move the cursor to the middle of the screen.

`L`                   move the cursor to the bottom of the screen.

`CTRL-f`              move the cursor forward by a screen of text

`CTRL-b`              move the cursor backward by a screen of text

`CTRL-u`              move the cursor up by half a screen

`CTRL-d`              move the cursor down by half a screen
___
### INSERT MODE

`i`                   start insert mode at cursor

`I`                   insert at the beginning of the line

`A`                   append at the end of the line

`a`                   append after the cursor

`O`                   open blank line above current line

`o`                   open (append) blank line below current line

`Esc`                 exit insert mode
___
### EDITING

`u`                   undo

`CTRL-r`              redo

`\>>`                  indent line one column to right

`==`                  auto-indent current line

`<<`                  indent line one column to left

`J`                   join line below to the current one

`cc`                  change (replace) an entire line

`ddp`                 swap current line with next

`ddkp`                swap current line with previous
___
### DELETING TEXT

`x`                   delete current character

`X`                   delete previous character

`dw`                  delete the current word

`dd`                  delete (cut) a line

`D`                   delete from cursor to end of line

`:[range]d`           delete [range] lines
___
### COPYING AND MOVING TEXT

`yw`                  yank word

`yy`                  yank (copy) a line

`2yy`                 yank 2 lines

`y$`                  yank to end of line

`p`                   put (paste) the clipboard after cursor/current line

`:set paste`          avoid unexpected effects in pasting

`\>`                   shift right

`<`                  shift left
___
### VISUAL MODE

`v`                   start visual mode, mark lines, then do command (such as y-yank)

`V`                   start linewise visual mode

`CTRL-v`              start visual block mode

`ab`                  a () block (with braces)

`ab`                  a {} block (with brackets)

`ib`                  inner () block

`ib`                  inner {} block

`v%`                  selects matching parenthesis

`vi{`                 selects matching curly brace

`vi"`                 selects text between double quotes

`vi'`                 selects text between single quotes
___
### EXITING

`:q`                  quit Vim. This fails when changes have been made.

`:q!`                 quit without writing.

`ZZ`                  write current file, if modified, and exit.

`:wq`                 write the current file and exit.

`:wq {file}`          write to {file}. Exit if not editing the last

`:[range]wq[!]`       same as above, but only write the lines in [range].
___
# SEARCH/REPLACE

`/pattern`                    search for pattern

`?pattern`                    search backward for pattern

`n`                           repeat search in same direction

`N`                           repeat search in opposite direction

`\*`                           search forward, word under cursor

`\#`                           search backward, word under cursor

`:%s/old/new/g`               replace all old with new throughout file

`:%s/old/new/gc`              replace all old with new throughout file with confirmation

`:argdo %s/old/new/gc | wq`   open multiple files and run this command to replace old 
                            with new in every file with confirmation, save and quit
___
### WINDOWS

`:sp f`               split open f

`:vsp f`              vsplit open f

`CTRL-w s`            split windows

`CTRL-w w`            switch between windows

`CTRL-w T`            move the current split window into its own tab

`CTRL-w q`            quit a window

`CTRL-w v`            split windows vertically

`CTRL-w x`            swap windows

`CTRL-w h`            left window

`CTRL-w j`            down window

`CTRL-w k`            up window

`CTRL-w l`            right window

`CTRL-w +`            increase window height

`CTRL-w -`            decrease window height

`CTRL-w <`            increase window width

`CTRL-w >`            decrease window width

`CTRL-w =`            equal window

`CTRL-w o`            close other windows
___
### TABS

`:tabnew file`        open a file in a new tab

`gt|:tabnext|:tabn`   move to the next tab

`gT|:tabprev|:tabp`   move to the previous tab

`:tabmove #`          move current tab to the #th position (indexed from 0)

`:tabclose|:tabc`     close the current tab and all its windows

`:tabonly|:tabo`      close all tabs except for the current one

`:tabdo command`      run the command on all tabs (e.g. :tabdo q - closes all opened tabs)
___
### PLUGINS > CHEAT
`:Cheat`              open cheat sheet (with autocomplete)

`<leader>ch`          open cheat sheet for word under the cursor
