# Bandit Level 0 → 1

## Objective

The objective of this level is to connect to `bandit.labs.overthewire.org` on port `2220` using SSH and retrieve the password for the next level.

**Username:** `bandit0`

## Skills Practiced

* Linux command line
* SSH
* File navigation
* Reading file contents

## Commands Used

```bash
ssh      # Connect to a remote system
ls       # List files and directories
cat      # Display the contents of a file
```

## Explanation

### Step 1: Learn about SSH

Before connecting, I read the SSH manual using:

```bash
man ssh
```

This helped me understand the purpose of the command and some of its commonly used options.

### Step 2: Connect to the server

Use SSH to connect to the Bandit server with the correct username and port.

### Step 3: List the files

After logging in successfully, list the files in the current directory. A file named `readme` is present.

### Step 4: Read the file

Display the contents of the `readme` file to obtain the password for the next level.

### Step 5: Exit

After completing the challenge, disconnect from the SSH session.

## Key Takeaways

* Learned how to connect to a remote Linux machine using SSH.
* Practiced using `ls` to inspect a directory.
* Used `cat` to read the contents of a file.
* Learned that Linux manual pages (`man`) are a valuable resource for understanding commands.

## Resources

* OverTheWire Bandit
* Linux manual pages (`man`)
* Built-in help (`--help`)

## Full Walkthrough

A detailed walkthrough with screenshots, command explanations, and the complete solution is available on my blog.

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-0-1-walkthrough)