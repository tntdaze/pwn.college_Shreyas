# Practicing Piping

## Split-piping stderr and stdout
In this challenge, you have:

/challenge/hack: this produces data on stdout and stderr
/challenge/the: you must redirect hack's stderr to this program
/challenge/planet: you must redirect hack's stdout to this program
Go get the flag!

### Solve
**Flag:** `pwn.college{Y6zg2VA2kF6Dgh8S4CZAo5YmoUt.QXxQDM2wiNzAzNzEzW}`

In this challenge, ```tee 2>``` which is for redirecting stderr to the given file ```/challenge/the``` and used ```tee 1>``` which is used for redirecting stdout to the file ```/challenge/planet``` and got the flag.

```bash
 /challenge/hack | tee 2>(/challenge/the) | tee 1>(/challenge/planet)
```

### New Learnings
Learned about split piping for errors and outputs.
