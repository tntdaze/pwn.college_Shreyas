# File Globbing

## Matching with *
Starting from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag!

### Solve
**Flag:** `pwn.college{opJJo44j0mbiV1OENeDZrXg622D.QXxIDO0wiNzAzNzEzW}`

In this challenge, I used cd command with ```/c*``` to change directory and then used ```/challenge/run``` to get the flag.

```bash
cd /c*
/challenge/run
```

### New Learnings
Learned about matching files with *.
