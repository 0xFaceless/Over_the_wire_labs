# Bandit Level 13 → 14

## Objective

Retrieve the password for Bandit Level 14. The password for the next level can be read from `/etc/bandit_pass/bandit14`, but only after logging in as `bandit14` using the private SSH key provided in the home directory.

**Username:** `bandit13`

## Skills Learned

- Understanding SSH key authentication
- Using a private SSH key
- Setting correct file permissions
- Reading protected files

## Commands Used

```bash
ssh
ls
cp
chmod
cat
man
```

## Key Takeaways

- SSH supports authentication using private keys.
- Private keys should have restrictive permissions (`600`).
- The `-i` option specifies the private key to use.
- `cat` can be used to read protected files after successful authentication.

## Blog

📖 Read the complete walkthrough on my blog.

[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-13-14-walkthrough)