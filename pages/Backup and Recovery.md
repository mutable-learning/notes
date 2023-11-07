tags:: Software Development
topic:: [[File Management]]
softdev:: Unit 4 Outcome 1

-
- important to have a backup and restore procedure in place for a software project to protect against data loss and corruption
- data loss can occur due to a variety of factors
	- natural disaster
	- hardware failure
	- software failure
	- human error
	- security failure
- developers and companies can recover from data loss quickly and easily if proper backup and recovery processes and procedures are in place
- Backup types
	- Full backup
		- copies all of the files in a software project to a backup location
		- is the most comprehensive type of backup, but it can also be the most time-consuming
		- takes up the most storage space
		- useful for creating a backup before a major release or before making a significant change to the project
	- Incremental backup
		- copies only the files that have changed since the last backup
		- a faster type of backup than a full backup, but it requires that a full backup exists
		- takes more time to restore: first full backup, then each incremental backup in order
		- a good option for backing up files that are changed frequently
	- Differential backup
		- copies only the files that have changed since the last full backup
		- a faster type of backup than an incremental backup, but it also requires that a full backup exist first
		- takes less time to restore: full backup then differential backup
		- a good option for backing up files that are changed infrequently
	- [[Version Control]]
		- allows developers to track changes to files and restore previous versions of files
		- a flexible way to back up and restore files
		- **not designed to be a primary backup solution**
		- a good option for recovering from accidental changes or for rolling back to a previous version of the project
- backups can also be used to create a test environment where the project can be safely tested without affecting live data
- a backup process is only as good as the restore process
	- check that backups are correctly made regularly
	- have a clear set of instructions for restoring systems from backup
	- periodically run the restoration process in an environment that resembles the live one as closely as possible
	- make sure backup media is protected from loss, damage and is stored securelylo