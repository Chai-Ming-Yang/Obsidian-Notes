Spaces are delimiters
```
[Command] [Option] [Parameters]
```

### `uniq`
`uniq -c logfile.log`
`-c` *count*

### **`sshd`**
Secure SHell Daemon

#### command substition
```
USERS = 'cmd_1' | `cmd_2` 
```

### **`sed`**
```
sed 's/find/replace/nth-occurence'

sed 's/find/replace/g'      # g : replaces all
```
- doesn't change file
- intercepts and modifies output
redirect operators are needed to actually modify file

### `sort`
`-r` *reverse*
`-u` *unique*
`-c` *check sorted*
`-o` *output into file*
`-u` *user_sort*
`-M` *month_sort*
`-n` *numerical_sort*
`-k` *kth_col_sort*

### **`awk`**
- *script lang*
- generate formatted report
	- text processing  &  pattern scanning
`-F` : *field separator*
`-f` : *src file*
`-v` : `var=value`
`$2` : *2nd field*

### **`tee`**
output to **file** & **stdout**

### `cut`
`-b <numByte>`   1-4
`-c <numCol>`     `-2` : *`[:2]`*      `3-5` : *`[3:5]`*      `6-` *`[6:]`*
`-f <numField>`
`-d <delim>`


### `noclobber`
`set -o noclobber`
- don't overwrite existing files
- prompts error