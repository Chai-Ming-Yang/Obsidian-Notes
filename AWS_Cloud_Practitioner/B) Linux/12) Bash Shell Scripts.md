Shell Script : 
- text files
- sequence of command
- automated by cron
Benefit: Automation remove human error
1. create script
2. set perms execute
3. `./` to run  
	- if  `.sh`  not in $PATH


**Automation Examples**
- Backup
- Move old files (only newest visible)
- Find duplicate files

## Characters
|          |                                                                                    |
| -------- | ---------------------------------------------------------------------------------- |
| **`#`**  | comment (ignored)                                                                  |
| **`#!`** | *shebang* <br>instructs what to execute with<br>can run directly<br>`#! /bin/bash` |

## Commands
|              |                                     |
| ------------ | ----------------------------------- |
| **`echo`**   | outpu                               |
| **`read`**   | input                               |
| **`subStr`** | get substr                          |
| **`+`**      | add / concat                        |
| **`file`**   | open file                           |
| **`mkdir`**  | create dir                          |
| **`cp`**     | copy                                |
| **`mv`**     | move / rename                       |
| **`chmod`**  | mod perms<br>`chmod +x`             |
| **`rm`**     | del                                 |
| **`ls`**     | list                                |
| **`grep`**   |                                     |
| **`find`**   |                                     |
| ``` ` ` ```  | substitution<br>``` "hi `name`" ``` |
## Params
|                      |                                                             |
| -------------------- | ----------------------------------------------------------- |
| **`$0`**             | script (path/name)                                          |
| **`$1`**             | 1st - 9th arg                                               |
| **`${10}`**          | 10th arg ++                                                 |
| **`$@`**<br>**`$*`** | all args                                                    |
| **`$?`**             | exit status *(previous cmd)*<br>`0` : success<br>`1` : fail |
| **`read`**           | input to var<br>`read varname`                              |
| **`exit`**           | `exit 0`<br>`exit 1`                                        |

## Conditionals
| **`if[  ]; then `**<br>	*`code`*<br>**`elif[  ]; then `**<br>	*`code`*<br>**`else`**<br>	*`code`*<br>**`fi`**<br><br> |
| --------------------------------------------------------------------------------------------------------------------- |
| **`case`**<br><br>                                                                                                    |

# Boolean

|                         |                                      |
| ----------------------- | ------------------------------------ |
| **`true`**              |                                      |
| **`false`**             |                                      |
| **`-Z`**                | Zero Len str                         |
| **`-n`**                | not null                             |
| **`-eq`**<br>**`==`**   | equal                                |
| **`!=`**                | not equal                            |
| **`-gt`**<br>**`>`**    | greater than                         |
| **`-lt`**<br>**`<`**    | less than                            |
| **`-ge`**<br>**`>=`**   | greater equal                        |
| **`-le`**<br>**`<=`**   | less equal                           |
| **`[ ]`**<br>**`test`** | POSIZ-compliant (sh, dash, bash)<br> |
| **`[[ ]]`**             | Bash, Zsh, Ksh extension             |

## Loops
| **`for`***`x in 1 2 3 a b c`***`; do`** <br>	*`code`*<br>**`done`**<br><br>                        |
| -------------------------------------------------------------------------------------------------- |
| **`while [`** *`condition`* **`]; do`**<br>	`code`<br>**`done`**<br><br>                           |
| *`counter = 1`*<br>**`until [`** *`counter -gt 10`* **`]; do`**<br>	*`code`*<br>**`done`**<br><br> |
| `break`<br><br>                                                                                    |
| `continue`<br><br>                                                                                 |
