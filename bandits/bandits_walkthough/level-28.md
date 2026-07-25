# Bandit Level 28 → Level 29

## Level Goal

The password for the next level is hidden in the Git repository's commit history.

## Steps

### 1. View the README

```bash
cat README.md
```

The password was replaced with `XXXXXXXXXX`, so it was no longer visible.

### 2. View the commit history

```bash
git log
```

Output:

```text
commit e2e1de5...  fix info leak
commit 2678cfa...  add missing data
commit 9530d52...  initial commit
```

The latest commit mentioned **"fix info leak"**, suggesting the password existed in an earlier commit.

### 3. Checkout the previous commit

```bash
git checkout 2678cfadd**********************
```

Git entered **detached HEAD** mode.

### 4. Read the README again

```bash
cat README.md
```

Output:

```text
# Bandit Notes

Some notes for level29 of bandit.

## credentials

username: bandit29
password: <bandit29 password>
```

The password for the next level was revealed.

## Commands Used

```bash
cat README.md

git log

git checkout 2678cfadd8f2a34**********************

cat README.md
```

## Concepts Learned

- Git commit history
- `git log`
- `git checkout <commit>`
- Detached HEAD state
- Recovering previous versions of files