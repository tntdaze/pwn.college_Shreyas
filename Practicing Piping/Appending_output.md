# Practicing Piping

## Appending output
To practice, run /challenge/run with an append-mode redirect of the output to the file /home/hacker/the-flag. The practice will write the first half of the flag to the file, and the second half to stdout if stdout is redirected to the file. If you properly redirect in append-mode, the second half will be appended to the first, but if you redirect in truncation mode (>), the second half will overwrite the first and you won't get the flag!

### Solve
**Flag:** `pwn.college{4p4OYbzlG6oxPOwvY_SmWIZovIh.QX3ATO0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```>>``` to redirect the given file in append mode and used ```cat``` command on it to read the file and got the flag.

```bash
/challenge/run >> /home/hacker/the-flag
cat the-flag
```

### New Learnings
Learned about appending output.
