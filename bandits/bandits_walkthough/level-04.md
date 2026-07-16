# Bandit Level 4 → 5

## Objective

Retrieve the password for Bandit Level 5. The password is stored in the only human-readable file inside the `inhere` directory.

**Username:** `bandit4`

## Skills Learned

- Identifying file types
- Using the `file` command
- Handling filenames beginning with `-`
- Reading text files

## Commands Used

```bash
ssh
cd
ls
file
cat
```

## Key Takeaways

- The `file` command identifies a file's type based on its contents.
- Filenames beginning with `-` require special handling.
- Both `file -- *` and `file ./*` correctly identify the file types.
- Once the human-readable file is identified, `cat` can be used to display its contents.

## Blog

📖 Read the complete walkthrough:

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-4-5-walkthrough)