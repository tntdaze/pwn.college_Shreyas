# Data Manipulation

## Extracting the first lines with head
This challenge's /challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college, which will give you the flag if you do this right! Your solution will be a long composite command with two pipes connecting three commands.

### Solve
**Flag:** `pwn.college{AA8xaFwQtCBIELVj2YxlbE7dyYz.0lNxEzNxwiNzAzNzEzW}`

In this challenge, I used ```/challenge/pwn``` with ```head -n 7``` to only print the first 7 lines and used pipe operator to pipe it on to ```/challenge/college``` and got the flag.

```bash
/challenge/pwn | head -n 7 | /challenge/college
```

### New Learnings
Learned about extracting specific lines.
