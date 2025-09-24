# Digesting Documentation

## Helpful Programs
In this level, you will practice reading a program's documentation with --help. Try it out!

### Solve
**Flag:** `pwn.college{IJCgIRHocjM6R31brN0q-TVXFTU.QX3IDO0wiNzAzNzEzW}`

In this challenge, I used ```--help``` argument on /challenge/challenge which printed this:
```bash
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
```
I used ```-p``` argument to get the value and used ```-g 631``` and got the flag.

```bash
/challenge/challenge --help
/challenge/challenge -p
/challenge/challenge -g 631
```

### New Learnings
Learned about reading a program's documentation with --help.
