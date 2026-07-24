# Bandit Level 24 → 25

## Objective

The objective of this level is to connect to a service running on localhost port `30002` and brute-force a 4-digit PIN along with the current Bandit24 password to retrieve the password for Bandit25.

## Skills Practiced

- Netcat (`nc`)
- Bash for loops
- Brute-force automation
- Output redirection
- Using `uniq`

## Commands Used

```bash
nc      # Connect to TCP service
for     # Loop through values
echo    # Print text
uniq    # Remove consecutive duplicate lines
```

## Explanation

### Step 1

Connect to the service running on localhost port `30002` using Netcat.

### Step 2

Read the instructions printed by the service. It asks for the current password followed by a 4-digit PIN separated by a space.

### Step 3

Instead of manually trying every PIN, use a Bash `for` loop to generate all values from `0000` to `9999`.

### Step 4

Send every password and PIN combination to the service using Netcat.

### Step 5

Redirect the output into a file.

### Step 6

Use `uniq` (or `grep "Correct!"`) to locate the successful response.

### Step 7

The service prints the password for Bandit25.

## Key Takeaways

- Learned how to automate repetitive tasks using Bash loops.
- Practiced using Netcat to communicate with TCP services.
- Understood output redirection.
- Learned a simple brute-force technique.

## Resources

- OverTheWire Bandit
- Linux manual pages (`man nc`)
- Bash documentation

## Full Walkthrough

A detailed walkthrough with screenshots and explanations is available on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/bandit-level-24-25-walkthrough-brute-forcing-a-pin-with-bash)