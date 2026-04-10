most servers use Linux
- GUI is optional
- information stored as text files (even though not `.txt`)
	- Light-weight
	- Save cost (less storage)
- 

# Vim Commands
VimTutor to learn Vim
- ./vimtutor
## Command Mode
|                                          |                                                                              |
| ---------------------------------------- | ---------------------------------------------------------------------------- |
| **`dd`**                                 | Del Line                                                                     |
| **`U`**                                  | Undo                                                                         |
| **`i`**<br>**`A`**<br>**`o`**<br>**`O`** | Insert mode<br>- append at end of line<br>- newline below<br>- newline above |
| **`x`**                                  | Del Char                                                                     |
| **`ZZ`**                                 | **Save** & **Exit**                                                          |
| **`G`**                                  | Cursor EOF                                                                   |
| **`gg`**                                 | Cursor BOF                                                                   |
| **`42G`**                                | Go Line 42                                                                   |
| **`/`**                                  | Search                                                                       |
| **`y`**                                  | Yank (cut)                                                                   |
| **`p`**                                  | Put (paste)                                                                  |

## Insert Mode
|           |                    |
| --------- | ------------------ |
| **`Esc`** | Enter command mode |
--INSERT--
press escape to go back to Command mode
## Execute Mode
|            |                                                                                                                                                                                         |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`:w`**   | Writes (save)                                                                                                                                                                           |
| **`:q`**   | Quit Vim                                                                                                                                                                                |
| **`:wq`**  | Write (save) & Quit                                                                                                                                                                     |
| **`:wq!`** |                                                                                                                                                                                         |
| **`:q!`**  | Quit without saving changes                                                                                                                                                             |
| **`:s`**   | Substitute (replace)<br>`:s/old/new/`       (first char)<br>`:s/old/new/g`     (current line only)<br>`:%s/old/new/g`   (entire file)<br>`:%s/old/new/gc` (entire file w. confirmation) |
|            |                                                                                                                                                                                         |
**`:`** enter execute mode



# GNU nano Commands
|          |                    |
| -------- | ------------------ |
| `^G`     | Get  Help          |
| `^X`     | Close              |
| `^O`     | Open               |
| `^J`     | Justify            |
| **`^R`** | Read               |
| `^W`     | Where (search)     |
| `^Y`     | Prev Pg            |
| `^V`     | Nex Pg             |
| `^K`     | Cut (current line) |
| `^U`     | Uncut              |
| `^C`     | Cursor Pos         |
| **`^T`** | To spell           |
|          |                    |
|          |                    |

# Gedit
"**GUI** text editor"
- only available if GUI is installed
- menu buttons available