# Backup Script Guide

## Full Code of backup.sh
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
##  What Did the chmod +x Command Do?

The `chmod +x backup.sh` command gives the script permission to run. After this, we can execute it using `./backup.sh`.

## Cron Schedule
Cron expression:

```cron
0 2 * * * /root/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | At minute zero |
| Hour | 2 | At 2 AM |
| Day of Month | * | Every day of the month |
| Month | * | Every month |
| Day of Week | * | Every day of the week |

This Cron job runs the backup script every day at 2:00 AM.
