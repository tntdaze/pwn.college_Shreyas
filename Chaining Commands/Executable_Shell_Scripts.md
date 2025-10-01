# Chaining Commands

## Executable Shell Scripts
Make a shellscript that will invoke /challenge/solve, make it executable, and run it without explicitly invoking bash!

### Solve
**Flag:** `pwn.college{UzG4KH8JYPdnB0eQRDOIawotcC5.QX0cjM1wiNzAzNzEzW}`

In this challenge, I ran used ```echo``` with argument ```/challenge/solve``` onto ```x.sh``` and invoked ```chmod u=rwx``` on the file and ran ```/home/hacker/x.sh``` and got the flag.

```bash
echo "/challenge/solve" > x.sh
chmod u=rwx x.sh
/home/hacker/x.sh
```

### New Learnings
Learned about executing shell scripts.
