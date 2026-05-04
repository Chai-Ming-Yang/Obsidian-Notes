`TAR`
**`-f`** archives the files (tar can also archive devices).
**`-v`** is the everbose option to display what is put into the archive.
**`-z`** compresses the archive into the .gzip format.
**`tar -cf`** would work perfectly but would not display what is inside the archive and would not compress it.

| Symbolic Mode                                                                                                                                          | Absolute Mode                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| u (user)<br>g (group)<br>o (others)<br><br>`r` *(read)*<br>`w` *(write)*<br>`e` *(execute)*<br><br>`+` *(grant)*<br>`-` *(remove)*<br>`=` *(reassign)* | `700`<br><br>digits:<br>1st user<br>2nd group<br>3rd others<br><br>`1`: **e**      `2`: **w**<br>`3`: ew   `4`: **r**<br>`7` -- rwx<br> |

**`chmod 400 filename`**
- only owner can read

**`chown newOwner:newGroup filename`**
**`chown newOwner filename`**
**`chown :newGroup filename`**

# Principle of Least Permissions
