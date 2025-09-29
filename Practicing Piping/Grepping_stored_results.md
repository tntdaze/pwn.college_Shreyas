# Practicing Piping

## Grepping stored results
In preparation for more complex levels, we want you to:

Redirect the output of /challenge/run to /tmp/data.txt.
This will result in a hundred thousand lines of text, with one of them being the flag, in /tmp/data.txt.
grep that for the flag!

### Solve
**Flag:** `pwn.college{EFKDAjXtrhbblaKsaASBiPwWkID.QX4EDO0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```>``` and redirected output to the given file and then I used grep command to find the string ```pwn.college``` and gave the file as argument and got the flag.

```bash
/challenge/run > /tmp/data.txt
grep pwn.college /tmp/data.txt
```

### New Learnings
Learned about grepping stored results inside files.
