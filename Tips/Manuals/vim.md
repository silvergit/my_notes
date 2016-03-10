# Vim manual

---
## Modes

| Key   | Mode      |  
|-------|-----------|
| `i`   | Insert    |
| `Esc` | Normal    |
| `v`   | Visual    |

---
## Move

| Key   | Result                                        |
|-------|-----------------------------------------------|
| `h`   | Left                                          |
| `l`   | Right                                         |
| `j`   | Up                                            |
| `k`   | Down                                          |
| `%`   | Jump to the matching parenthesis or bracket   |
| `0`   | Beginning of a line                           |
| `$`   | End of a line                                 |
| `gg`  | Beginning of a file                           |
| `G`   | End of a file                                 |

---
## Insert

| Key           | Result                        | Sample            |
|---------------|-------------------------------|-------------------|
| `n`i`text`    | Insert `text` for `n` times   | `3iok` -> `okokok`|
| `o` or `O`    | Insert a new line after or before this line |     |

---
## Copy and Move text
| Key       | Result            |
|-----------|-------------------|
| `yy`      | Yank line         |
| `yy` `n`  | Yank `n` lines    |
| `p`       | Put the text      |

---
## Delete

| Key           | Result                |
|---------------|-----------------------|
| `d` `e`       | Delete the first word |
| `d` `n` `e`   | Delete the n words    |
| `d` `d`       | Delete line           |

---
## Search

| Key               | Result                | Sample            |
|-------------------|-----------------------|-------------------|
| `/` `word`        | Find next `word`      |                   |
| `/` `word` `Ctrl` | Highlight all `word`s |                   |
| `n` or `N`        | Repeat the search for next and previous occurrences | |

---
# Selecting text (Visual mode)
| Key   | Result    |
|-------|-----------|
| `d`   | Delete    |
| `y`   | Yank      |
| `>`   | Indent    |
| `<`   | Unindent  |

---
# Files

| Key           | Result                        |
|---------------|-------------------------------|
| `:w`          | Save                          |
| `:q`          | Quit                          |
| `:q!`         | Quit without saving           |
| `:u`          | Undo                          |
| `:red`        | Redo                          |
| `Ctrl` `R`    | Redo                          |
| `.`           | Repeat the previous command   |
| `:help`       | help                          |
