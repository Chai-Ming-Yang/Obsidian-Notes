## File: /etc/passwd
mmajor:x:524538:584731::/home/mmajor/:bin/bash
[User]   [UID]        [GID]      [home dir]        [default shell]

### '#' vs '$'
hash code means root user, no warnings for commands
### Benefit of **SUDO**
- administrative work.
- aware of what's done
- password authentication per 15 minutes
- trackable which non-admin called sudo


| Root User                                                           | Standard User                                |
| ------------------------------------------------------------------- | -------------------------------------------- |
| Full permission Every file<br>- rwx<br>(files == user/service/data) | Permission for files                         |
| Manage Linux kernel                                                 | Limited access to system                     |
| ```[root@server00 ~]#```<br><br>the '`#`' sign                      | ```[user@server ~]$```<br><br>the '`$`' sign |

|             |                                    |
| ----------- | ---------------------------------- |
| `su root`   | switch to root<br>current user env |
| `su - root` | switch to root<br>root user env    |


# `/etc/sudoers`

`%user localhost=/usr/sbin/shutdown -r now`


manage group of similar permission users together.
