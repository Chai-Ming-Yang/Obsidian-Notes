/etc/passwd
/etc/group


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
| **`ls`**      | List files in wd                                                             |
| **`touch`**   | **create** new empty file<br>update file timestamps                          |
| **`cat`**     | **read** data  from file<br>**contcatenate**                                 |
| **`find`**    |                                                                              |
| **`head`**    |                                                                              |
| **`grep`**    | search for string in file<br>grep "search_string" "source"                   |
|               |                                                                              |


# SUDO Commands
| **sudo**     | SuperUserDO (root user)<br>normal user doing administrative permission tasks                                                                                                                          |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **su**       | Promote to root user                                                                                                                                                                                  |
| **useradd**  | Add user of username<br>`-c` (comment about user)<br>`-e` (expiry date of user)<br>`-d` (set home directory of user)                                                                                  |
| **usermod**  | Modify existing user<br>`-l` (rename user)<br>`-aG` (append user to new group & keeping in old)<br>*"adding user to group is modify user, not group"*<br>`-L` (lock account)<br>`-U` (unlock account) |
| **userdel**  | Delete user<br>`-r` (also delete user's home directory)                                                                                                                                               |
| **passwd**   | Set password of user                                                                                                                                                                                  |
|              |                                                                                                                                                                                                       |
| **groupadd** | Create new Group<br>                                                                                                                                                                                  |
| **groupmod** | Modify existing group<br>                                                                                                                                                                             |
| **groupdel** | Delete Group<br>                                                                                                                                                                                      |
| **sudoers**  |                                                                                                                                                                                                       |
| **cut**      | filter<br>`-d`*c* [delimiter] separates by 'c'<br>`-f`*n,m,...* [field nth] show fields                                                                                                               |
|              |                                                                                                                                                                                                       |
|              |                                                                                                                                                                                                       |
|              |                                                                                                                                                                                                       |
|              |                                                                                                                                                                                                       |

# Modifier / Options
|     |                               |
| --- | ----------------------------- |
| -i  | perform case-sensitive search |
| -s  | shortened version             |
| -p  | pretty (human readable)       |
| -H  | table column headers          |
| -a  | all                           |
| -l  | long format                   |
| -m  | append                        |
| -d  | delimiter                     |
|     |                               |


# Operation Symbols

|     |                                                            |
| --- | ---------------------------------------------------------- |
| \|  | pipe symbol<br>redirect output of previous command to next |
|     |                                                            |