# Bandit Level 31 → Level 32

## Goal

Push a file named `key.txt` containing the exact text below to the remote Git repository:

```text
May I come in?
```

## Commands Used

```bash
ls
cat README.md

echo "May I come in?" > key.txt

git status
ls -la
cat .gitignore

rm .gitignore

git status
git add .
git commit -m "Solved Level 31"
git push
```

## Concepts Learned

- Hidden files can affect Git's behaviour.
- `.gitignore` prevents matching files from being tracked.
- `ls -la` is useful for discovering hidden configuration files.
- Always check `git status` before committing.