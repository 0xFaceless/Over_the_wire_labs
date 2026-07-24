# Bandit Level 23 → 24

## Objective

The objective of this level is to understand how a cron job executes scripts automatically and use it to retrieve the password for Bandit Level 24.

## Skills Practiced

- Linux cron jobs
- Reading shell scripts
- Bash scripting
- File and directory permissions
- Troubleshooting

## Commands Used

```bash
cat      # Display file contents
mkdir    # Create directory
touch    # Create file
nano      # Edit file
chmod    # Change permissions
cp       # Copy files
```

## Explanation

### Step 1

Navigate to `/etc/cron.d` and inspect the cron configuration.

### Step 2

Open the cron configuration file and identify the script being executed.

### Step 3

Read the shell script to understand how it works.

### Step 4

Create your own working directory under `/tmp`.

### Step 5

Create a shell script that copies `/etc/bandit_pass/bandit24` into a file inside your `/tmp` directory.

### Step 6

Initially, I only changed the permissions of the script using `chmod 777 f.sh`, but the cron job did not execute it successfully.

After troubleshooting, I recursively changed the permissions of the entire working directory using:

```bash
chmod -R 777 /tmp/jaiho
```

After that, the cron job executed the script successfully.

### Step 7

Copy the script into `/var/spool/bandit24/foo`.

### Step 8

Wait for about one minute and read the output file containing the password.

## Key Takeaways

- Learned how Linux cron jobs work.
- Practiced reading shell scripts written by others.
- Understood that directory permissions are just as important as file permissions.
- Learned how to troubleshoot permission-related issues.

## Resources

- OverTheWire Bandit
- Linux manual pages (`man cron`, `man chmod`, `man bash`)

## Full Walkthrough

A detailed walkthrough with screenshots and explanations is available on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/bandit-level-23-24-walkthrough-exploiting-a-cron-job)