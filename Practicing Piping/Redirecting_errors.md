# Practicing Piping

## Redirecting errors
Let's put this into practice! In this challenge, you will need to redirect the output of /challenge/run, like before, to myflag, and the "errors" (in our case, the instructions) to instructions. You'll notice that nothing will be printed to the terminal, because you have redirected everything! You can find the instructions/feedback in instructions and the flag in myflag when you successfully pull this off!

### Solve
**Flag:** `pwn.college{M6afjzTqTlit4IXiEzbMbuVK_h6.QX3YTN0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with multiple ```>``` at the same time, one for output and one for errors and after that I used ```cat``` command on instructions and myflag file to get the flag.

```bash
/challenge/run 1> myflag 2> instructions
cat instructions
cat myflag
```

### New Learnings
Learned about redirecting errors.
