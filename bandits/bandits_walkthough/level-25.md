# Bandit Level 25 → Level 26

## Level Goal

Log in as bandit26 using the SSH private key found in the home directory. The challenge is that bandit26 does not use a normal shell.

## Steps

### 1. Find the SSH key

```bash
ls
```

Output:

```text
bandit26.sshkey
```

### 2. Check bandit26's login shell

```bash
grep bandit26 /etc/passwd
```

Output:

```text
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext
```

### 3. Read the custom shell

```bash
cat /usr/bin/showtext
```

```bash
#!/bin/sh

export TERM=linux
exec more ~/text.txt
```

### 4. Login using the key

```bash
chmod 600 bandit26.sshkey

ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220
```

### 5. Keep `more` open

Resize the terminal so the text does not fit on one screen. This prevents `more` from exiting immediately.

### 6. Escape to Bash

Inside `more`:

```text
v
```

Inside Vim:

```vim
:set shell=/bin/bash
:shell
```

### 7. Read the password

```bash
cat /etc/bandit_pass/bandit26
```

## Concepts Learned

- Custom login shells
- `/etc/passwd`
- Reading shell scripts
- `more`
- Vim shell escape
- SSH private key authentication

