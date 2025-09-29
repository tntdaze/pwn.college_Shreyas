# Processes and Jobs

## Suspending Processes
This level's run wants to see another copy of itself running and using the same terminal. How? Use the terminal to launch it, then suspend it, then launch another copy while the first is suspended!

### Solve
**Flag:** `pwn.college{sks0RfTaoAuB9irh3S9cjENPm1q.QX1QDO0wiNzAzNzEzW}`

In this challenge, I ran ```/challenge/run``` then hit ctrl+z and used the command again which printed the flag.

```bash
/challenge/run
ctrl+z
/challenge/run
```

### New Learnings
Learned about suspending processes.
