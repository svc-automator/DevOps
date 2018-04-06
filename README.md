# DevOps
Home for all operations automation scripts

Molivero - add clean-backups.ps1 .  This script will check D:\Backup for backup folders created during deployments.  The current folder naming scheme includes a four digit year - e.g. 2018.  The script explictly only manages folders that contain a "20" in the folder name, so its only good for another 80 years.  Regardless of the name and whether the yyyy if first, last or embedded in the middle - it will scan all folders with a "20" - sort them by last write date, scan through them, keep the two most current and recursively dump the rest of them.
