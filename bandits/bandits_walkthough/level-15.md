# Bandit Level 15 → 16

## Objective

Retrieve the password for Bandit Level 16. Submit the current level's password to a service listening on `localhost` port `30001` using an SSL/TLS connection.

**Username:** `bandit15`

## Skills Learned

- Understanding SSL/TLS connections
- Using OpenSSL's `s_client`
- Sending data to secure network services

## Commands Used

```bash
ssh
man
openssl
```

## Key Takeaways

- `openssl s_client` connects to SSL/TLS-enabled services.
- Some network services require encrypted communication instead of plain TCP.
- The current password must be submitted after establishing the secure connection.
- Reading manual pages helps discover useful subcommands.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-15-16-walkthrough)