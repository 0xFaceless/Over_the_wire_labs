# Bandit Level 27 → Level 28

## Level Goal

Clone the Git repository and find the password for the next level.

## Steps

### 1. Clone the repository

Initially, I tried:

```bash
git clone ssh://bandit27-git@bandit.labs.overthewire.org/home/bandit27-git/repo
```

This failed because Git attempted to connect using the default SSH port (22).

The Bandit server uses **port 2220**, so I cloned the repository using:

```bash
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
```

### 2. Enter the repository

```bash
cd repo
```

### 3. List the files

```bash
ls
```

Output:

```text
README
```

### 4. Read the README

```bash
cat README
```

Output:

```text
The password to the next level is:
y8Yd2ss*********************
```

## Commands Used

```bash
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo

cd repo

ls

cat README
```

## Concepts Learned

- Git clone over SSH
- SSH default port (22)
- Specifying a custom SSH port
- Reading repository contents