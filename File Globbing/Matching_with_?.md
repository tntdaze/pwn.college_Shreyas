# File Globbing

## Matching with ?
Starting from your home directory, change your directory to /challenge, but use the ? character instead of c and l in the argument to cd! Once you're there, run /challenge/run for the flag!

### Solve
**Flag:** `pwn.college{cVrKU7VMmF9afz7mV4dYnuq1e4f.QXyIDO0wiNzAzNzEzW}`

In this challenge, I used cd command with ```/challenge``` and replaced ```c``` and both the ```l``` with ```?``` to get the flag.

```bash
cd /?ha??enge
/challenge/run
```

### New Learnings
Learned about matching files with ?.
