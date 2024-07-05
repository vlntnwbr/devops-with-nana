# Command Mode
- cannot write new content
- can navigate through the text and has cmds to manipulate it

# Insert / Edit Mode
- actually write new text

## How to exit Vim
- :wq -> save and close
- :q -> quit
- :q! -> force quit without saving changes

## Useful Commands (in command modes)
1. `dd` -> delete line
    - `d[n]` -> delete n number of lines (remove angle brackets)
2. `u` -> undo last change
3. `A` -> move to end of line and activate insert mode
4. `$` -> move to end of line without activating insert mode
5. `0` -> move to start of line without activating insert mode
6. `[n]G` -> jump to line [n] (remove angle brackets)
7. `/<pattern>` -> search for pattern in text (highlights first match)
    - `n` -> go to next occurrence
    - `N` -> go to previous occurrence 
8. `:%s/pattern/replacement` -> replace pattern with replacement
