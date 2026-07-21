# Bandit Level 16 → 17

## Objective

Retrieve the password for Bandit Level 17. Scan localhost for the correct SSL-enabled service, submit the current password, receive a private SSH key, and use it to log in as `bandit17`.

**Username:** `bandit16`

## Skills Learned

- Port scanning with Nmap
- Identifying network services
- Using OpenSSL to connect to SSL services
- SSH key authentication
- Reading protected files

## Commands Used

```bash
nmap
openssl
ssh
chmod
cat
```

## Key Takeaways

- `nmap` can discover open ports and identify running services.
- `openssl s_client` communicates with SSL/TLS-enabled services.
- SSH private keys should have restrictive permissions (`600`).
- SSH key authentication is commonly used instead of passwords.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-16-17-walkthrough)