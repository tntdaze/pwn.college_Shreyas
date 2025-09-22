# Pondering Paths

## home sweet home
In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
Again, you must specify your path as an argument to /challenge/run.

### Solve
**Flag:** `pwn.college{sV4GGnyUt_XkZLCfq3qfCkeEeBT.QXzMDO0wiNzAzNzEzW}`

In this challenge, At first, I used ```/challenge/run``` command with argument as ```~``` which didn't return any flag. Then, I used ```~/~``` as argument and got the flag.

```bash
/challenge/run ~/~
```

### New Learnings
Learned about the home directory ~ and its absolute path.
