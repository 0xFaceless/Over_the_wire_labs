# Bandit Level 26 → Level 27

## Level Goal

The goal is to obtain the password for **bandit27**.

## Steps

Since we already escaped the restricted shell in the previous level, we now have a Bash shell as **bandit26**.

A SUID binary named `bandit27-do` is available, which allows executing commands as **bandit27**.

Run:

```bash
./bandit27-do cat /etc/bandit_pass/bandit27
```

Output:

```text
STJL************************
```

## Commands Used

```bash
./bandit27-do cat /etc/bandit_pass/bandit27
```

## Concepts Learned

- Reusing access gained from the previous level
- SUID executables
- Reading protected files