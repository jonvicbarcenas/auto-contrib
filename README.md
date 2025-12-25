# GitHub Auto Commit

Automates daily GitHub contributions to maintain your green streak.

## Setup

1. Create a new GitHub repository
2. Clone it and copy these files into it
3. Run `git init` if needed, then set your remote

## Usage

Run manually:
```bash
npm run commit
```

## Automate with Task Scheduler (Windows)

1. Open Task Scheduler
2. Create Basic Task → Name it "GitHub Auto Commit"
3. Trigger: Daily at your preferred time
4. Action: Start a program
   - Program: `node`
   - Arguments: `index.js`
   - Start in: `C:\path\to\this\folder`

## Automate with Cron (Linux/Mac)

Add to crontab (`crontab -e`):
```bash
0 9 * * * cd /path/to/repo && node index.js
```

This runs daily at 9 AM.
