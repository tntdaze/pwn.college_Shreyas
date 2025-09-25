# File Globbing

## Mixing globs
Now, let's put the previous levels together! We put a few happy, but diversely-named files in /challenge/files. Go cd there and, using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!

### Solve
**Flag:** `pwn.college{EGU2H5nuPEDnDV7uAK3octl_X-C.QX1IDO0wiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```/challenge/files``` first then tried using ```c*e*p*``` and the terminal gave an error saying square bracket glob missing. Then, I tried using ```[cep*]``` which also didn't work and then I realized it should be []* since * file glob would try to fill in the characters after the first character so ```[cep]*``` worked to get the flag.

```bash
cd /challenge/files
/challenge/run [cep]*
```

### New Learnings
Learned about mixing file globs.
