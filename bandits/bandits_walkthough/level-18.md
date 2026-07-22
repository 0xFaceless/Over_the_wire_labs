# Bandit Level 18 → 19

## Objective

Retrieve the password for Bandit Level 19. The shell logs you out immediately because `.bashrc` has been modified, so execute a command remotely over SSH instead of opening an interactive shell.

**Username:** `bandit18`

## Skills Learned

- Remote command execution with SSH
- Understanding SSH command syntax
- Bypassing interactive shell restrictions

## Commands Used

```bash
man
ssh
cat
ls
```

## Key Takeaways

- SSH can execute a command directly on a remote host.
- Remote commands do not require an interactive shell.
- `cat` can be used to display the password stored in a file.
- Reading manual pages reveals useful SSH features.

## Blog

📖 Read the complete walkthrough on my blog.
[Walkthrough](https://0xfaceless.hashnode.dev/overthewire-bandit-level-18-19-walkthrough)