# File Globbing

## Matching with []
We've placed a bunch of files in /challenge/files. Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!

### Solve
**Flag:** `pwn.college{4-1tKzFeQTAyPiZ05UXpecwah9A.QXzIDO0wiNzAzNzEzW}`

In this challenge, I changed directory to ```/challenge/files``` then used ```/challenge/run``` with argument ```file_[bash]``` by using the first character of each file to get the flag.

```bash
cd /challenge/files
/challenge/run file_[bash]
```

### New Learnings
Learned about matching files with [].
