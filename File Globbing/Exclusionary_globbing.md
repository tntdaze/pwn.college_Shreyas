# File Globbing

## Exclusionary globbing
Armed with this knowledge, go forth to /challenge/files and run /challenge/run with all files that don't start with p, w, or n!

### Solve
**Flag:** `pwn.college{YeWelPmP6K_HB8cZd-4PUpLfZJU.QX2IDO0wiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```/challenge/files``` first then used the argument ```[!pwn]*``` with run command since the file shouldn't start with either of the letters and * is there to cover all file names that are longer than one character which start with either of the three letters.

```bash
cd /challenge/files
/challenge/run [!pwn]*
```

### New Learnings
Learned about mixing file globs.
