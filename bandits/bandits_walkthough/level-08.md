# Bandit Level 8 → 9

## Objective

Retrieve the password for Bandit Level 9. The password is stored in the file `data.txt` and is the only line that occurs once.

**Username:** `bandit8`

## Skills Learned

- Sorting text with `sort`
- Finding unique lines with `uniq`
- Using pipes (`|`) to combine commands

## Commands Used

```bash
ssh
ls
man
uniq
sort
```

## Key Takeaways

- `uniq` only detects adjacent duplicate lines.
- `sort` groups identical lines together.
- Pipes (`|`) allow the output of one command to become the input of another.
- `sort data.txt | uniq -u` prints only the lines that appear once.

## Blog

📖 Read the complete walkthrough:

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-8-9-walkthrough)