# Practicing Piping

## Grepping errors
The shell has a >& operator, which redirects a file descriptor to another file descriptor. This means that we can have a two-step process to grep through errors: first, we redirect standard error to standard output (2>& 1) and then pipe the now-combined stderr and stdout as normal (|)!

### Solve
**Flag:** `pwn.college{E7eduFsjhJ2tAYxl25eFxDChE3G.QX1ATO0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```2>& 1``` as given in the instructions to redirect standard error but it didn't print the flag then I realized I had to use the pipe operator too for grepping the flag with string ```pwn.college```. 

```bash
/challenge/run 2>& 1 | grep pwn.college
```

### New Learnings
Learned about grepping errors.
