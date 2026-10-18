# Mission 9: The Cloud Automation Engineer

## Mission Overview

This mission focuses on automating backup tasks using Bash scripts and Cron. It helps create backups automatically without running commands manually every time.

## Objectives

- Understand basic Bash scripting.
- Create and run a backup script.
- Use chmod to change file permissions.
- Schedule tasks using Cron.
- Document the process using Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```
## Skills Learned

-Writing and running Bash scripts.
-Creating backup files.
-Using Linux file permissions.
-Scheduling tasks automatically.
-Creating Markdown documentation.
