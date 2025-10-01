# Pondering PATH

## Adding Commands
Previously, the win command that /challenge/run executed was stored in /challenge/more_commands. This time, win does not exist! Recall the final level of Chaining Commands, and make a shell script called win, add its location to the PATH, and enable /challenge/run to find it!

### Solve
**Flag:** `pwn.college{EKUKxYVw_4SxsDrG-FsmfECXlgv.QX2cjM1wiNzAzNzEzW}`

In this challenge, I typed ```echo $PATH``` and saw a list of directories and one by one checked if it had cat inside using ```ls``` and found it in ```/usr/bin```. I added a ```win``` file with the text ```/usr/bin/cat /flag```. Next, I added it to the path using ```PATH="$PWD:$PATH"``` and got the flag.

```bash
echo $PATH
nano win
/usr/bin/cat /flag
PATH=$"PWD:$PATH"
/challenge/run
```

### New Learnings
Learned about adding commands.
