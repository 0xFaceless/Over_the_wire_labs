# Bandit Level 12 → 13

## Objective

Retrieve the password for Bandit Level 13. The password is stored in `data.txt`, which is a hexadecimal dump of a file that has been repeatedly compressed.

**Username:** `bandit12`

## Skills Learned

- Working in a temporary directory
- Reversing a hexadecimal dump
- Identifying file types
- Decompressing archives
- Extracting tar archives

## Commands Used

```bash
ssh
mkdir
cp
cd
xxd
file
mv
gzip
gunzip
bzip2
tar
cat
```

## Key Takeaways

- `xxd -r` converts a hexadecimal dump back into its original binary format.
- Always identify a file before extracting it using the `file` command.
- Different archive formats require different extraction tools.
- Some files contain multiple layers of compression.

## Blog

📖 Read the complete walkthrough on my blog.

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-12-13-walkthrough)