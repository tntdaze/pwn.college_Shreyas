# Practicing Piping

## Duplicating piped data with tee
This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

### Solve
**Flag:** `pwn.college{8-3Z32mS-RNOtwoM84h34O-Gh5U.QXxITO0wiNzAzNzEzW}`

In this challenge, I used ls command to see which data file needs to be read and typed ```cat data.txt``` which gave a [SECRET ARG] and I piped ```/challenge/pwn``` into ```/challenge/college``` using the ```|``` operator and got the flag. 

```bash
ls
cat data.txt
/challenge/pwn --secret 8-3Z32mS | /challenge/college
```

### New Learnings
Learned about duplicating piped data with tee.
