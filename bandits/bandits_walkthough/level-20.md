# Bandit Level 20 → 21

## Objective

Retrieve the password for Bandit Level 21 by using the `suconnect` program. The program connects to a TCP port on localhost and expects the current level's password before returning the next password.

**Username:** `bandit20`

## Skills Learned

- Netcat (`nc`)
- TCP client/server communication
- Linux job control (`Ctrl + Z`, `fg`, `jobs`)
- Localhost networking

## Commands Used

```bash
./suconnect
nc
jobs
fg
```

## Key Takeaways

- `nc` can be used to create a simple TCP server.
- `suconnect` acts as a TCP client.
- Job control allows multiple terminal processes to be managed.
- Programs can communicate through localhost.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-20-21-walkthrough)