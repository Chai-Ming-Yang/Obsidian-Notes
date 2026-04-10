### Editable Text Configuration
"/etc/.psswd"
colon (:) separated fields
- User name or Login name
- Encrypted passwords
- User ID  &  Group ID
- User description
- User's home directory
- User's login shell

### Login Workflow
1. **user name** checked against **/etc/passwd**
	- name field max == 32 chars
	- No-Capitalization (good practice)
2. **password** checked against **/etc/shadow**
	- pass
3. **Load** files from user's home dir
	- home/username/.bashrc
	- home/username/.bash_history
	- home/username/.bash_profile
4. 

|            |                                            |
| ---------- | ------------------------------------------ |
| **stdin**  | incoming data (input devices)<br>value 0   |
| **stdout** | outgoing data (write data/apps)<br>value i |
| **stderr** | redirect to logs file<br>value 2           |




