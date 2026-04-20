Program -- series of instructions *(for computer)*
- **System Program** *(native)*
	- Primal computer function
	- Operating system commands
	- Does not interface with the user
- **Application Program** *(external)*
	- Comprehensive program
	- Perform specific function
	- Can be used by another user

`$path`
- each process assigned PID *Process ID*

**Process == Running Program**
Life Cycle : 'Start' --> (Ready/Running/Waiting) --> 'Stopped'
- "waiting" : for event
- "ready"    : to be assigned processor time

Complex Application require `>1 child processes`
- inherit most of parent attribute

|              |                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **`ps`**     | Process status<br>PID<br>TTY *(terminal type)*<br>Runtime *(duration)*<br>CMD *(that launched process)*<br>`-e` everything<br>`-f` formatted<br>`-b` batch mode<br>`-p` PID select<br>`-a` filter *(not associated with terminal)*<br>`-T` filter *(associated with terminal)*<br>`-r` filter *(running)*<br>`L`   Lightweight Processes *(threads)*<br>`\| grep sshd`  *Ssh Daemon* |
| **`pidof`**  | PID of file<br>`pidof [program]`<br>`pidof sshd`<br>`pidof bash`<br>`-s` single *(return 1 PID)*<br>`-c` common *(same root dir)*<br>`-w` wider *(flexible name match)*<br>`-S` separator *(between PIDs)*                                                                                                                                                                           |
| **`pstree`** | tree format *`ps`*<br>`[]` process          `{}` child process<br>`-a` include args<br>`-p` include PID<br>`-c` nc<br>`-n` numerical *(slow execution) (clear order)*                                                                                                                                                                                                                |
| **`top`**    | Task Manager<br>"running" <br>"sleep" -- waiting for I/O<br>"stopped" -- being traced / stopped by job control signal<br>"zombie" -- child of ended process<br>`-h` *help section*<br>`-v` *version*<br>`-b` batch mode *(non-interactive)*                                                                                                                                          |
|              |                                                                                                                                                                                                                                                                                                                                                                                      |

CPU Values in `top`

| value | description                            |
| ----- | -------------------------------------- |
| us    | run duration in **user space**         |
| sy    | run duration in kernel space processes |
| id    | idle duration                          |
| wa    | wait duration *(I/O)*                  |
| hi    | duration handle hardware problems      |
| si    | duration handle software problem       |
| st    | steal duration *(by other processes)*  |



| `at` | `cron` |
| ---- | ------ |
|      |        |
