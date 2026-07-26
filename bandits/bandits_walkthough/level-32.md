# Bandit Level 32 → Level 33

## Goal

Escape the restricted shell and retrieve the password for Bandit Level 33.

## Commands Used

```bash
$0

cat /etc/bandit_pass/bandit33
```

## Concepts Learned

- Restricted shells limit the commands you can execute.
- `$0` starts the user's default shell.
- Once inside the normal shell, standard Linux commands become available.
- Environment variables can sometimes be used to bypass restricted shells.

