# Backup Script Guide

## Full Code of backup.sh

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

##  What Did the chmod +x Command Do?

The `chmod +x backup.sh` command gives the script permission to run. After this, we can execute it using `./backup.sh`.

## Cron Schedule
Cron expression:

```bash
0 2 * * * /root/backup.sh

- *Minute:* 0 – Runs at minute zero.
- *Hour:* 2 – Runs at 2:00 AM.
- *Day of Month:* * – Runs every day of the month.
- *Month:* * – Runs every month.
- *Day of Week:* * – Runs every day of the week.

This Cron job runs the backup script every day at 2:00 AM.
