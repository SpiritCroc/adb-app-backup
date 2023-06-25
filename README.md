# ADB app backup

Backup apps to your PC using adb root.
No extra apps or app root required.

Supports multiple devices and multiple backups per app.


## Examples

View available options

`python3 adbappbackup --help`

View available backups

`python3 adbappbackup`

### Backup

Backup a single app

`python3 adbappbackup --backup com.example.app`

Get a list of apps to backup

`python3 adbappbackup --list_packages > my_apps.txt`

Backup the list of apps

`python3 adbappbackup --package_list my_apps.txt --backup`


### Restore

Restore a single app

`python3 adbappbackup --restore com.example.app`

Restore a list of apps

`python3 adbappbackup --package_list my_apps.txt --restore`

Restore latest app backup from a different device

`python3 adbappbackup --backup_device SERIAL --restore com.app.packagename --latest`


### Clean up old backups

Delete all backups except the latest 5 for each app

`python3 adbappbackup --keep 5`
