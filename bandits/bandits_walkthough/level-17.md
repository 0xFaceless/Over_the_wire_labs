# Bandit Level 17 → 18

## Objective

Retrieve the password for Bandit Level 18. Compare `passwords.old` and `passwords.new` to find the only changed password.

**Username:** `bandit17`

## Skills Learned

- Comparing files
- Using the `diff` command
- Identifying changed lines

## Commands Used

```bash
ls
diff
```

## Key Takeaways

- `diff` compares two files line by line.
- Lines beginning with `<` belong to the first file.
- Lines beginning with `>` belong to the second file.
- The changed line in `passwords.new` is the password for the next level.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-17-18-walkthrough)