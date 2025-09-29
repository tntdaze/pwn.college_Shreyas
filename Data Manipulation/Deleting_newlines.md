# Data Manipulation

## Deleting newlines
Now, let's combine this with deletion. In this challenge, we'll inject a bunch of newlines into the flag. Delete them with tr's -d flag and the escaped newline specification!

### Solve
**Flag:** `pwn.college{EUpMv4z0n9sFDdkM379V3hjTiSn.0VNxEzNxwiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```tr``` command and  ```-d "\n"``` which removed the newlines and printed the flag.

```bash
/challenge/run | tr -d "\n"
```

### New Learnings
Learned about deleting newlines.
