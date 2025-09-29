# Practicing Piping

## Redirecting more output
Aside from redirecting the output of echo, you can, of course, redirect the output of any command. In this level, /challenge/run will once more give you a flag, but only if you redirect its output to the file myflag. Your flag will, of course, end up in the myflag file!

### Solve
**Flag:** `pwn.college{MyTuHE1RyLSCIqw0Lx6aOtGQEub.QX1YTN0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```>``` on the given file which gave the output file which contained the flag which I used ```cat``` command to get the flag.

```bash
/challenge/run > myflag
cat myflag
```

### New Learnings
Learned about redirecting more output.
