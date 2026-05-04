
|          |                                               |
| -------- | --------------------------------------------- |
| `$PATH`  | Environmental Path **CRITICAL**<br>           |
| `$SHELL` | Default Shell                                 |
| `$HOME`  |                                               |
| `$USER`  | Current Username <br>(reassigned upon reopen) |

1. User Logs In
2. Default system shell starts
3. Run `etc/profile`
4. ``
5. ``
6. `.bashrc`


```
#! /bin/bash
name=$1
counter=$(
        ls "${name}"* 2>/dev/null \
                | sed -E "s/^${name}//" \
                | grep -E '^[0-9]+$' \
                | sort -n \
                | tail -1
)

if [ -z "$counter" ]; then
        counter=0
fi

for ((i=counter; i<=counter+25; i++)); do
        touch "${name}${i}"
done
```

