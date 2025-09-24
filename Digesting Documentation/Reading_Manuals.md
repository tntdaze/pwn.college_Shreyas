# Digesting Documentation

## Reading Manuals
The challenge in this level has a secret option that, when you use it, will cause the challenge to print the flag. You must learn this option through the man page for challenge!

### Solve
**Flag:** `pwn.college{k8BpiGYgBS2mbsBtSEfXaAdPylj.QX0EDO0wiNzAzNzEzW}`

In this challenge, I used ```man challenge``` to get the manual and saw one of the descriptions as ```--kpigmb NUM``` prints flag if NUM is 820 so I used it with ```/challenge/challenge``` and got the flag.

```bash
man challenge
/challenge/challenge --kpigmb 820
```

### New Learnings
Learned about reading manuals and its usage.
