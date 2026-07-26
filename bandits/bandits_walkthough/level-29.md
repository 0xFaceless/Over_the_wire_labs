# Bandit Level 29 → Level 30

## Level Goal

Find the password for **bandit30** by exploring the Git repository.

## Solution

Read the README.

```bash
cat README.md
```

The password is hidden.

View all commits and branches.

```bash
git log --all
```

Notice the `dev` branch.

Checkout the commit pointed to by the `dev` branch.

```bash
git checkout 0bf8160435c51*************************
```

Read the README again.

```bash
cat README.md
```

The password for **bandit30** is displayed.

## Commands Used

```bash
cat README.md

git log --all

git checkout 0bf816043**************************

cat README.md
```

## Concepts Learned

- `git log --all`
- Git branches
- `git checkout`
- Detached HEAD