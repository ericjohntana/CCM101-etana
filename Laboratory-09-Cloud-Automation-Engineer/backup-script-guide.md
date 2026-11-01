# Backup Script Guide 

## 1. Overview

This documentation explains the Bash backup script created for Laboratory 9. The script automatically compresses the application data directory and stores the backup file inside a separate `backups` directory.

A timestamp is included in the backup filename to identify when each backup was created.

## 2. Full Bash Script

The following is the complete Bash script used in this activity:

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

## 3. Explanation of the Script

| Command or Variable | Description |
|---|---|
| `#!/bin/bash` | Specifies Bash as the interpreter used to execute the script. |
| `SOURCE_DIR="app-data"` | Defines the directory containing the application data to be backed up. |
| `BACKUP_DIR="backups"` | Defines the directory where backup files will be stored. |
| `TIMESTAMP=$(date +"%Y%m%d_%H%M%S")` | Generates the current date and time for the backup filename. |
| `echo` | Displays messages in the terminal. |
| `mkdir -p $BACKUP_DIR` | Creates the backup directory if it does not already exist. |
| `tar -czf` | Creates a compressed `.tar.gz` archive of the source directory. |

## 4. File Permissions and Execution

Initially, executing the script using the following command resulted in a permission-denied error:

```bash
./backup.sh
```

To allow the script to execute, the following command was used:

```bash
chmod +x backup.sh
```

The `chmod` command changes file permissions, while `+x` adds executable permission to the file. After applying this permission, the script could be executed using:

```bash
./backup.sh
```

The script successfully created the `backups` directory and generated a compressed backup file.

### Backup Verification

The following command was used to verify the generated backup:

```bash
ls -l backups/
```

Actual backup file created during the activity:

```text
backup_20261101_060857.tar.gz
```

## 5. Cron Job Configuration

A Cron job was configured to automatically execute the backup script every day at 2:00 AM.

The Cron expression used was:

```bash
0 2 * * * /root/backup.sh
```

### Breakdown of the Five Cron Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Runs at minute zero. |
| Hour | `2` | Runs at 2:00 AM. |
| Day of Month | `*` | Runs every day of the month. |
| Month | `*` | Runs every month. |
| Day of Week | `*` | Runs every day of the week. |

### Cron Schedule Explanation

- **Minute:** `0` – The task starts at minute zero.
- **Hour:** `2` – The task runs at 2:00 AM.
- **Day of Month:** `*` – The task runs every day.
- **Month:** `*` – The task runs every month.
- **Day of Week:** `*` – The task runs every day of the week.
- **Command:** `/root/backup.sh` – Specifies the Bash backup script to execute.

### Cron Configuration Commands

The following commands were used to configure and verify the Cron job:

```bash
crontab -l
env EDITOR=nano crontab -e
crontab -l
```

The final `crontab -l` command displayed the installed schedule:

```bash
0 2 * * * /root/backup.sh
```

## 6. Screenshots

### Backup Script Execution

This screenshot shows the permission-denied attempt, the execution permission command, the successful backup script execution, and the generated compressed backup file.

![Backup Script Execution](screenshots/Checkpoint%204%20-%20script-execution.png)

### Cron Schedule Configuration

This screenshot shows the installed Cron schedule for automatically running the backup script every day at 2:00 AM.

![Cron Schedule Configuration](screenshots/Checkpoint%205%20-%20cron-schedule.png)

## 7. Lesson Learned

This activity demonstrated how Bash scripting, Linux file permissions, and Cron scheduling can be used together to automate backup tasks. The backup script successfully compressed the sample application data into a `.tar.gz` file, while the Cron job was configured to execute the script automatically every day at 2:00 AM. These techniques help reduce repetitive manual work and support consistent data backup in cloud environments.
