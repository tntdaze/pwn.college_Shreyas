# Shell Variables

## Reading Files
Now, use that to read /challenge/read_me into the PWN environment variable, and we'll give you the flag! The /challenge/read_me will keep changing, so you'll need to read it right into the PWN variable with one command!

### Solve
**Flag:** `pwn.college{Yp8w63miYSP-_bfCzWRU7_cPDXy.QXwIDO0wiNzAzNzEzW}`

In this challenge, I used read command with ```PWN < /challenge/read_me``` and got the flag.

```bash
read PWN < /challenge/read_me
```

### New Learnings
Learned about reading files.
