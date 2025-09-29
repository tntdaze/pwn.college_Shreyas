# Perceiving Permissions

## Executable Files
In this challenge, the /challenge/run program will give you the flag, but you must first make it executable!

### Solve
**Flag:** `pwn.college{gToG5EDOjp2OV3_HnjtQv2a3uY9.QXyEjN0wiNzAzNzEzW}`

In this challenge, I used ```ls -l``` on ```/challenge/run``` and saw that execute permission wasn't given to user since hacker here is the root. So, I used ```chmod``` with ```u+x``` to give the execute access to hacker and got the flag.

```bash
ls -l /challenge/run
chmod u+x /challenge/run
/challenge/run
```

### New Learnings
Learned about changing file permissions.
