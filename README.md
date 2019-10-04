# ADB app backup

Backup apps to your PC using adb root.
No extra apps or app root required.

Supports multiple devices and multiple backups per app.


## Examples

View available options

`adbappbackup --help`

View available backups

`adbappbackup`

### Backup

Backup a single app

`adbappbackup --backup com.example.app`

Get a list of apps to backup

`adbappbackup --list_packages > my_apps.txt`

Backup the list of apps

`adbappbackup --package_list my_apps.txt --backup`


### Restore

Restore a single app

`adbappbackup --restore com.example.app`

Restore a list of apps

`adbappbackup --package_list my_apps.txt --restore`
