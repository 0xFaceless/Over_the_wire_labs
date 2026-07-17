# Bandit Level 6 → 7

## Objective

Retrieve the password for Bandit Level 7. The password is stored somewhere on the server and has the following properties:

- Owned by user `bandit7`
- Owned by group `bandit6`
- 33 bytes in size

**Username:** `bandit6`

## Skills Learned

- Searching the filesystem with `find`
- Filtering by owner, group, and file size
- Redirecting error output

## Commands Used

```bash
ssh
find
cat
```

## Key Takeaways

- `find` can search the entire filesystem using multiple conditions.
- Permission denied messages are written to **stderr**.
- Redirecting stderr to `/dev/null` keeps the output clean.

## Blog

📖 Read the complete walkthrough:

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-6-7-walkthrough)