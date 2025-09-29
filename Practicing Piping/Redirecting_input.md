# Practicing Piping

## Redirecting input
You can do interesting things with a lot of different programs using input redirection! In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE! To write that value to the PWN file, recall the prior challenge on output redirection from echo!

### Solve
**Flag:** `pwn.college{QPOBNjRFc6mvJeZ2vYNnYkeCxBg.QXwcTN0wiNzAzNzEzW}`

In this challenge, I used echo command to write COLLEGE into PWN file. Then, I used ```<``` to read the PWN file and followed the instructions to get the flag.

```bash
echo COLLEGE > PWN
/challenge/run < PWN
```

### New Learnings
Learned about redirecting input.
