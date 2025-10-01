# Terminal Multiplexing

## Detaching and Attaching
For this challenge, you'll need to:

Launch screen
Detach from it.
Run /challenge/run (this will secretly send the flag to your detached session!)
Reattach to see your prize

### Solve
**Flag:** `pwn.college{Q6HjkF8E_DoA_fmpYD8gd-zl_Z3.0lN4IDOxwiNzAzNzEzW}`

In this challenge, I launched the screen using ```screen``` command and detached using ```ctrl+a -d``` and then attached using ```screen -r``` and got the flag.

```bash
screen
ctrl+a -d
/challenge/run
screen -r
```

### New Learnings
Learned how to detach and attach screen.
