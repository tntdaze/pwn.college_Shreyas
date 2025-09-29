# Practicing Piping

## Process substitution for input
This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

### Solve
**Flag:** `pwn.college{oUMf7Hp4sxOK7hgyIROh4ZSaa6q.0lNwMDOxwiNzAzNzEzW}`

In this challenge, I used diff command on both file paths using ```<``` to get the flag.

```bash
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
```

### New Learnings
Learned about process substitution.
