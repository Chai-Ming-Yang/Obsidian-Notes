
| Method           |                                                                                                                                                                            |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RedHat           | **RedHat Package Manager (RPM)**<br>- `.rpm` packages<br>- `YUM` interface with RPM<br>- track package dependency<br>- auto-update<br>*e.g. Amazon Linux 2 , RedHat Linux* |
| Debian           | **dpkg**<br>- `.deb` extension<br>- `APT` interface<br>*e.g. Debian , Ubuntu*                                                                                              |
| Install from src | **CNU Compiler Collection (GNU)**<br>"human readable" --> "machine"<br>"compiled" --> installed                                                                            |

## Package Managers
Maintain software through life cycle
- Install  ,  Update  ,  Inventory  ,  Uninstall
Package software
- precompiled-code  ,  documentation  ,  installation-instruction

## Repositories
*e.g. Vendor Server, Internal Server, Hard Disk*
- Repo available to PM is defined in config file
- Amazon Linux 2 repo : "amzn2-core"  "amzn2extra-docker"

## `yum`
`-y` yes to all confirmation
**`yum install`**` <package-name>`
**`yum update`**`  <package-name>`
**`yum remove`**`  <package-name>`
**`yum list installed`**

#### install from src
1. Download src pkg *(tarball)*
2. Unarchive pkg   **`tar -xzf`**` <filename.tar.gz>`
3. Compile src    *(GCC)*
4. Install software

## File Retrieval
| `wget`                                      | `curl`                       |
| ------------------------------------------- | ---------------------------- |
| - recursive download                        | - single rsc only            |
| - support HTTP/HTTPS/FTP                    | - support HTTP/HTTPS/FTP/... |
| - Perform retries *(unreliable connection)* | - run on more platform       |

```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

unzip awscliv2.zip
sudo ./aws/install
```
`-o` : output file name
