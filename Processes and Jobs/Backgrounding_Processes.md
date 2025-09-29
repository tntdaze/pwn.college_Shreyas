# Processes and Jobs

## Backgrounding Processes
This level's run wants to see another copy of itself running, not suspended, and using the same terminal. How? Use the terminal to launch it, then suspend it, then background it with bg and launch another copy while the first is running in the background!

### Solve
**Flag:** `pwn.college{8T9kTYBbwaCndmNZODrsf_3Rqva.QX3QDO0wiNzAzNzEzW}`

In this challenge, I ran ```/challenge/run``` then hit ctrl+z and used the ```bg``` command and typed ```/challenge/run``` again which printed the flag.

```bash
/challenge/run
ctrl+z
bg
/challenge/run
```

### New Learnings
Learned about backgrounding processes.
