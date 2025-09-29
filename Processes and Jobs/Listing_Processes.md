# Processes and Jobs

## Listing Processes
In this level, I have once again renamed /challenge/run to a random filename, and this time made it so that you cannot ls the /challenge directory! But I also launched it, so you can find it in the running process list, figure out the filename, and relaunch it directly for the flag! Good luck!

### Solve
**Flag:** `pwn.college{0nuwu87oo49tw1fHb5jriWoRrki.QX4MDO0wiNzAzNzEzW}`

In this challenge, I used ```ps aux``` and identified the challenge file and ran it to get the flag.

```bash
ps aux
/challenge/8356-run-32420
```

### New Learnings
Learned about listing processes.
