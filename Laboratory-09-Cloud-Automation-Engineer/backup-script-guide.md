# Backup Script Guide

## The Script (backup.sh)

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## What did chmod +x do?

The `chmod +x backup.sh` command adds execute permission to the script. This allows Linux to run the file as a program when I enter `./backup.sh`. It is necessary because a script may not be executable when it is first created.

## Cron Expression

```bash
0 2 * * * /home/ccastillo/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | The task starts when the minute is zero. |
| Hour | 2 | The task is scheduled for the 2 AM hour. |
| Day of Month | * | The task can run on any date of the month. |
| Month | * | The task can run during any month of the year. |
| Day of Week | * | The task can run on any day of the week. |

This cron expression schedules the backup script to run every day at 2:00 AM. It helps the client maintain regular backups without depending on someone to remember to start the task.

The script should also be tested to make sure the source folder and backup folder are found correctly when cron runs it.
