# File Globbing

## Multiple globs
We put a few happy, but diversely-named files in /challenge/files. Go cd there and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p.

### Solve
**Flag:** `pwn.college{0ipxLiS_AGyBMskPC_AC64ZNhao.0lM3kjNxwiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```/challenge/files``` first then tried using ```/p**``` which gave an error saying argument is too long and then I realized the ```/``` took up an extra character as max limit was 3 after which I typed ```*p*``` and got the flag.

```bash
cd /challenge/files
/challenge/run *p*
```

### New Learnings
Learned about using multiple globs at the same time.
