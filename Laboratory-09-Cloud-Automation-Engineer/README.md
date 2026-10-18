# Laboratory 09: Cloud Automation Engineer

## Mission Overview

This laboratory activity introduced me to automating routine tasks in a Linux environment. I created a sample application directory and wrote a Bash script to compress its contents into a backup file. I also learned how to allow the script to execute and schedule it to run every night using cron.

## Objectives

* Learn the basic structure of a Bash script.
* Use variables to store directory names and other values.
* Create and compress a sample application data folder.
* Apply executable permission using the `chmod` command.
* Schedule a script using the Linux cron service.
* Document the activity and its results in the GitHub portfolio.

## Commands Executed

Create the sample application data:

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
```

Create and run the backup script:

```bash
nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
```

Check and configure the cron schedule:

```bash
crontab -l
env EDITOR=nano crontab -e
crontab -l
```

## Skills Learned

In this activity, I practiced creating a Bash script and using it to back up application data. I learned how to compress files, manage execution permissions, and check whether a backup file was created. I also practiced using cron to schedule a task for a specific time. These skills showed me how automation can reduce repetitive work and help maintain important files.

## Screenshots

The `screenshots/` folder contains the required evidence:

* `script-execution.png`
* `cron-schedule.png`
