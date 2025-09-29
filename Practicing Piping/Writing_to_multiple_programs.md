# Practicing Piping

## Writing to multiple programs
In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands!

### Solve
**Flag:** `pwn.college{A37EE-on0AB40m1679My6qkkAQW.QXwgDN1wiNzAzNzEzW}`

In this challenge, I used ```tee``` to duplicate output data on both the given files using ```|``` operator and got the flag.

```bash
/challenge/hack | tee >(/challenge/the) | tee >(/challenge/planet)
```

### New Learnings
Learned about writing to multiple programs.
