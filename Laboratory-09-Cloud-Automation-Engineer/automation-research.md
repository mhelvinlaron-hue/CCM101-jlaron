# Automation Research

## Bash Script

A Bash script is a text file that contains Linux commands arranged to complete a task. The `#!/bin/bash` line tells the system which program should interpret and run the commands in the file. It is useful when I need to perform several commands without typing each one separately.

## Variables

Variables hold values that a script uses while it is running. For example, `$BACKUP_DIR` represents the folder where the backup files will be placed, so I do not have to repeat the folder name throughout the script. If I decide to use another folder, I can change the variable value instead of editing every command.

## Cron Job

A cron job is a Linux feature that runs commands automatically at a scheduled time. It is useful for cloud engineers because they can schedule regular tasks, such as backing up application files, without having to start them manually. This helps keep important tasks running on a consistent schedule.
