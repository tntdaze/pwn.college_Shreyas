# Pondering Paths

## Position elsewhere
This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program.

### Solve
**Flag:** `pwn.college{AMQ7GkenayeP8jns_Fb4iisKOkP.QX3QTN0wiNzAzNzEzW}`

In this challenge, Firstly, I ran the ```/challenge/run``` command to know which path the flag is in. Then, I used ```cd /var/log``` to switch current working directory and ran the challenge command again to get the flag. 

```bash
/challenge/run
cd /var/log
/challenge/run
```

### New Learnings
Learned how to change directory and invoking absolute paths from there.
