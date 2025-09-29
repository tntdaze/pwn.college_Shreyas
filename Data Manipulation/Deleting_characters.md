# Data Manipulation

## Deleting characters
I'll intersperse some decoy characters (specifically: ^ and %) among the flag characters. Use tr -d to remove them!

### Solve
**Flag:** `pwn.college{wwYdtGQ3YvFzIqdKzABB1My-vMQ.0FNxEzNxwiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```-d ^%``` which removed the unwanted characters and printed the flag.

```bash
/challenge/run | tr -d ^%
```

### New Learnings
Learned about deleting characters.
