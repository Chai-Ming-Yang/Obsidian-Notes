"record events on system"

|             |                                          |
| ----------- | ---------------------------------------- |
| System      | startup / shutdown                       |
| Event       | login / logout                           |
| Application | startup time / actions *(user)* / errors |
| Service     |                                          |
## Importance
1. Security Audits
2. SLA (Service Level Agreements)
3. Proactive troubleshooting
4. Industry Requirements

`cat /var/log/error_log | grep ERROR`
`tail -f /var/log/yum.log | grep ERROR`
`cat /tmp/log/secure | grep LOGIN`

## Levels
|     |             |                               |
| --- | ----------- | ----------------------------- |
| `0` | `EMERGENCY` | **System** unstable           |
| `1` | `ALERT`     | Immediate **action** needed   |
| `2` | `CRITICAL`  | **Critical error** *unstable* |
| `3` | `ERROR`     | non-critical Error            |
| `4` | `WARN`      | Warnings                      |
| `5` | `NOTICE`    | Events                        |
| `6` | `INFO`      | Informational Messages        |
| `7` | `DEBUG`     | all debu-level                |

## Directory *(storage)*
```
/var/log
```
`/var`
- files **rapidly** / **unpredictably** change in size

|                               |                                            |
| ----------------------------- | ------------------------------------------ |
| `/var/log/syslog`             | System Info                                |
| `/var/log/lastlog`            | Success Logins                             |
| `/var/log/secure`             | Auth info *(RedHat distro)*                |
| `/var/log/auth.log`           | Auth info *(for Debian-derived distro)*    |
| `/var/log/kern`               | Kernel Info *(linux)*                      |
| `/var/log/boot.log`           | Startup messages                           |
| `/var/log/maillog`            | Mail messages                              |
| `/var/log/daemon.log`         | Background services                        |
| `/var/log/cron.log`           | Schedule tasks                             |
| `/var/log/httpd`              | Apache info *(RedHat distro)*              |
| `/var/log/YUM`                | Yum Installer info *(RedHat distro)*       |
| `/var/log/apache2/access.log` | Apache auth info *(Debian-derived distro)* |

### `lastlog`
`-u <username>` 
`-t <x-days-ago>` 


# Log Rotation
- Frequent logs from servers  -->  bulky log files
**`logrotate`**
- limit total-size of retained logs
