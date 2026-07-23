# Bandit Level 19 → 20

## Objective

Retrieve the password for Bandit Level 20. Use the SUID binary `bandit20-do` to execute a command as the `bandit20` user.

**Username:** `bandit19`

## Skills Learned

- Understanding SUID permissions
- Executing commands as another user
- Reading protected files

## Commands Used

```bash
ls
./bandit20-do
cat
```

## Key Takeaways

- SUID binaries execute with the permissions of the file owner.
- `bandit20-do` allows commands to run as the `bandit20` user.
- Protected files can be accessed through authorized SUID programs.
- Always inspect unknown binaries before using them.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-19-20-walkthrough)