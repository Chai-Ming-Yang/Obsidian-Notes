/etc/passwd
/etc/group
## Terminal

|               |                                                                              |
| ------------- | ---------------------------------------------------------------------------- |
| `whoami`      | Print current user name                                                      |
| `id`          | User & Group info                                                            |
| `hostname`    | Current system's host / domain / node name                                   |
| `date`        | datetime                                                                     |
| `cal`         | Calendar `-j` (Julian calendar)<br>`-s` (Sunday=1st)       `-m` (Monday=1st) |
| **`uptime`**  | Time since last boot (even in sleep / hibernation)                           |
| **`echo`**    | Print                                                                        |
| **`man`**     | manual                                                                       |
| **`!!`**      | rerun last command                                                           |
| **`clear`**   | Clear terminal                                                               |
| **`pwd`**     | Print Working Directory                                                      |
| **`history`** | History of commands<br>"/home/username/.bash_history"                        |
| **`ps`**      | Process Status<br>`-e` everything<br>`-f` full format<br>`-l` long format    |

## Navigation / Dir & Files

| **`ls`**    | List files in wd<br>`-l` long format<br>`-a` all (include hidden)<br>`-R` recursive<br>`-h` human readable<br>`-X` sort by extension<br>`-S`             size<br>`-t`             time modified<br>`-v`             version number |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`touch`** | **create** new empty file<br>update file timestamps                                                                                                                                                                                |
| **`cat`**   | **read** data  from file<br>**contcatenate**                                                                                                                                                                                       |
| **`more`**  | **Forward Scroll** (pages)<br>Read % of File *(slow on large file)*<br>`-d` *"press space to continue, 'q' to quit"*<br>`-f` no line wrap<br>`-p` *`clear`* before output<br>`-s` squeeze >1 blank line into 1                     |
| **`less`**  | **Forward & Backward Scroll** (pages)<br>Read enough to fill screen (same speed)<br>`-N`  show line numbers<br>`-X` not *`clear`* before output<br>`-F`                                                                            |
| **`head`**  | first 10 lines of file *(default)*<br>`-n` num lines to display<br>`-c` bytes to display                                                                                                                                           |
| **`tail`**  | last 10 lines of file *(default)*<br>`-f` Monitor File Change<br>`-n` num lines to display<br>`-c` bytes to display                                                                                                                |
| **`cd`**    | change directory<br>`../` move up 1 directory                                                                                                                                                                                      |
| **`grep`**  | search content in file<br>grep "search_string" "source"                                                                                                                                                                            |
| **`cp`**    | Copy<br>`-a` archive (preserve metadata)<br>`-f` force<br>`-i` interactive (confirmation)<br>`-n` no overwrite existing<br>`-l` **link** files<br>`-L` *follow* symbolic link<br>`-r` recursive<br>`-u` update<br>`-v` verbose     |
| **`mv`**    | Move / Rename<br>`-i` interactive (confirmation)<br>`-f` force<br>`-n` no overwrite existing<br>`-v` verbose                                                                                                                       |
| **`rm`**    | Remove<br>`-d` directory (empty dir)<br>`-r` Recursive<br>`-f` Force (no confirm msg)<br>`-i` interactive<br>`-v` visual (print files deleted)                                                                                     |
| **`mkdir`** | Make dir<br>`-m` Set permission to dir *`-m 400`*<br>`-p` create parent dir                                                                                                                                                        |

# Files

|                              |                                                                                                                                                                                                                                           |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`hash`**                   | hash table of recently executed programs<br>`-d` delete the location<br>`-l` output *(redirect to function)*<br>`-p` set path name<br>`-r` empty hash table<br>`-t` display location of command                                           |
| **`cksum`**                  | generate checksum *(check corruption)*<br>**workflow:**<br>1. *record* cksum result      *(before transfer)*<br>2. compare cksum result   *(upon receive)*                                                                                |
| **`find`**                   | search file and directories<br>`-name <fname>`<br>`-iname <fname>` *case insensitive*<br>`-user <uname>`<br>`-type <ftype>`<br>`-size <fsize>`<br>`-fprint` output location<br>`-exec` run command on searched file<br>`-delete` del file |
| **`grep`**                   | search content in file<br>`-i` ignore case<br>`-r` recursive<br>`-l` list only file name<br>`-n` display line num<br>`-c` count of matching                                                                                               |
| **`diff`**                   | display difference btw files<br>                                                                                                                                                                                                          |
| **`ln`**                     | create pointer to given file  *(hard link)*<br>`-s` soft link                                                                                                                                                                             |
| **`tar`**                    | **Combine** *without compression*<br>`-x` extract *tarball* content<br>`-z` compress content with **gzip**<br>`-f` specify name of tarball<br>`-v` verbose                                                                                |
| **`gzip`**                   | compress & decompress files *include tarballs*<br>`-d` decompress                                                                                                                                                                         |
| **`zip`**<br><br>**`unzip`** | compress file<br>`-r` recursive<br>extract                                                                                                                                                                                                |

# Services

|        |                                             |
| ------ | ------------------------------------------- |
| lscpu  | list CPU info                               |
| lshw   | list hardware                               |
| du     | disk used <br>check file & dir size         |
| df     | disk free<br>display disk size & free space |
| fdisk  | list & modify partition on hard drive       |
| vmstat | indicate use of virtual memory              |
| free   | indicate use of physical memory             |
| top    | taskmgr *(dynamic)*                         |
| uptime | duration since boot & num users             |

# SUDO Commands
| **`sudo`**      | SuperUserDO (root user)<br>normal user doing administrative permission tasks                                                                                                                                                                                                |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`su`**        | Promote to root user                                                                                                                                                                                                                                                        |
| **`useradd`**   | Add user of username<br>`-c` (comment about user)<br>`-e` (expiry date of user)<br>`-d` (set home directory of user)                                                                                                                                                        |
| **`usermod`**   | Modify existing user<br>`-l` (rename user)<br>`-aG` (append user to new group & keeping in old)<br>*"adding user to group is modify user, not group"*<br>`-L` (lock account)<br>`-U` (unlock account)                                                                       |
| **`userdel`**   | Delete user<br>`-r` (also delete user's home directory)                                                                                                                                                                                                                     |
| **`passwd`**    | Set password of user                                                                                                                                                                                                                                                        |
|                 |                                                                                                                                                                                                                                                                             |
| **`groupadd`**  | Create new Group<br>                                                                                                                                                                                                                                                        |
| **`groupmod`**  | Modify existing group<br>                                                                                                                                                                                                                                                   |
| **`groupdel`**  | Delete Group<br>                                                                                                                                                                                                                                                            |
| **`gpassword`** | Administer "/etc/group" file<br>`-a` `--add`                      (add user to group)<br>`-d` `--delete`                (remover user from group)<br>`-M` `--members`              (show member list of group)<br>`-A` `--administrators` (set administrator list of group) |
| **`sudoers`**   |                                                                                                                                                                                                                                                                             |
| **`cut`**       | filter<br>`-d`*c* [delimiter] separates by 'c'<br>`-f`*n,m,...* [field nth] show fields                                                                                                                                                                                     |
|                 |                                                                                                                                                                                                                                                                             |
|                 |                                                                                                                                                                                                                                                                             |
|                 |                                                                                                                                                                                                                                                                             |
|                 |                                                                                                                                                                                                                                                                             |

# Modifier / Options
|          |                               |
| -------- | ----------------------------- |
| **`-i`** | perform case-sensitive search |
| **`-s`** | shortened version             |
| **`-p`** | pretty (human readable)       |
| **`-H`** | table column headers          |
| **`-a`** | all *(include hidden)*        |
| **`-l`** | long format                   |
| **`-m`** | append                        |
| **`-d`** | delimiter                     |
| **`-R`** | List subdirectories           |
| **`-x`** |                               |


# Metacharacters

|                                 |                                                         |
| ------------------------------- | ------------------------------------------------------- |
| **`*`**                         | wildcard *(multi-char)*                                 |
| **`?`**                         | wildcard *(single-char)*                                |
| `[` charactes `]`               | matching chars<br>`[az]`   a or z<br>`[a-z]` a to z<br> |
| **``` `cmd` ```** or **`$cmd`** | command substitution                                    |
| **`;`**                         | chain commands tgt                                      |
| **`~`**                         | represent home dir                                      |
| **`-`**                         | represent previous work dir                             |

# Redirection
|     |                                         |
| --- | --------------------------------------- |
| >   | output to file                          |
| <   | receive input from file                 |
| \|  | redirect output (left) to input (right) |
| >>  | append output to file                   |
| 2>  | redirect error to file                  |
| 2>> | append error to file                    |


# FHS (File System Hierarchy) Standard
|          |                               |
| -------- | ----------------------------- |
| `/`      | Root                          |
| `/boot`  | Boot Files                    |
| `/dev`   | Devices                       |
| `/etc`   | Config                        |
| `/home`  | Stc. User's home dir          |
| `/media` | Removable Media               |
| `/mnt`   | Network drives                |
| `/root`  | **Root user** home dir        |
| `/var`   | Logs & network & print spools |


