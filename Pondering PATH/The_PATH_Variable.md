# Pondering PATH

## The PATH Variable
In this level, you will disrupt the operation of the /challenge/run program. This program will DELETE the flag file using the rm command. However, if it can't find the rm command, the flag will not be deleted, and the challenge will give it to you! Thus, you must make it so that /challenge/run also can't find the rm command!

### Solve
**Flag:** `pwn.college{sJPcO3lxzX9LfSbV7Nf6cQEdeNz.QX2cDM1wiNzAzNzEzW}`

In this challenge, I typed ```PATH=''``` and used ```/challenge/run``` and got the flag.

```bash
PATH=''
/challenge/run
```

### New Learnings
Learned about the PATH variable.
