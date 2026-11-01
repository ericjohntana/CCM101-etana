# Laboratory 9 – The Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on automating system administration tasks using Bash shell scripting and Linux Cron scheduling.

The activity involves creating a sample application data directory, writing a Bash script that automatically compresses and backs up the data, assigning executable permissions, and configuring a Cron job to run the backup automatically every night at 2:00 AM.

## Objectives

- Understand the fundamental syntax of a Bash shell script, including variables and basic commands.
- Use a command-line text editor (nano) to write and save executable scripts.
- Modify Linux file permissions using the chmod command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of your GitHub Cloud Computing Portfolio.

## Commands Executed

### 1. Check the Current Directory

```bash
pwd
```

Displays the current working directory in the Linux terminal.

### 2. Create the Application Data Directory

```bash
mkdir app-data
```

Creates a new directory named `app-data` to store the sample application data.

### 3. Create a Sample Data File

```bash
echo "This is critical client data." > app-data/data.txt
```

Creates a file named `data.txt` inside `app-data` and writes the sample client data into it.

### 4. Create the Bash Backup Script

```bash
nano backup.sh
```

Opens the Nano text editor to create and write the Bash backup script.

### 5. Attempt to Execute the Script

```bash
./backup.sh
```

Attempts to execute the backup script. The first attempt displays a `Permission denied` error because the script does not yet have executable permission.

### 6. Give the Script Executable Permission

```bash
chmod +x backup.sh
```

Adds executable permission to the backup script so it can be run as a program.

### 7. Execute the Backup Script

```bash
./backup.sh
```

Runs the backup script to create the backup directory and compress the application data into a `.tar.gz` file.

### 8. Verify the Generated Backup File

```bash
ls -l backups/
```

Displays the contents and file details of the `backups` directory to verify that the compressed backup file was created.

### 9. Check Existing Cron Jobs

```bash
crontab -l
```

Displays the current user's scheduled Cron jobs. Initially, no Cron configuration existed for root.

### 10. Open the Cron Configuration Editor

```bash
env EDITOR=nano crontab -e
```

Opens the Cron configuration file using the Nano text editor so a scheduled task can be added or modified.

### 11. Configure the Daily Backup Schedule

```bash
0 2 * * * /root/backup.sh
```

Schedules the backup script to run automatically every day at 2:00 AM. This line is added inside the Cron editor.

### 12. Verify the Installed Cron Schedule

```bash
crontab -l
```

Displays the installed Cron configuration to confirm that the daily backup schedule was successfully saved.

## Skills Learned

- **Bash Scripting:** Creating scripts to automate repetitive Linux commands.
- **Variables:** Storing and reusing directory paths and timestamp values.
- **File Management:** Creating directories and sample application data.
- **File Compression:** Using the `tar` command to create compressed backup archives.
- **File Permissions:** Using `chmod +x` to allow a script to execute.
- **Task Scheduling:** Configuring Cron jobs to run scripts automatically.
- **Technical Documentation:** Recording commands, configurations, and results using Markdown.
- **GitHub Portfolio Management:** Organizing and documenting laboratory activities in a GitHub repository.

## Screenshots

### 1. Backup Script Execution

This screenshot shows the successful execution of the Bash backup script and the generated compressed backup file.

![Backup Script Execution](screenshots/Checkpoint%204%20-%20script-execution.png)

### 2. Cron Schedule Configuration

This screenshot shows the installed Cron schedule configured to execute the backup script every day at 2:00 AM.

![Cron Schedule Configuration](screenshots/Checkpoint20%520%-20%cron-schedule.png)

---

Laboratory 9 demonstrated how Bash scripting, Linux file permissions, and Cron scheduling can work together to automate backup tasks. Through this activity, I successfully created a backup script that compresses application data into a `.tar.gz` file and configured a Cron job to run the script automatically every day at 2:00 AM.

This activity helped me understand how automation reduces repetitive manual work, improves consistency, and supports efficient cloud system administration.
