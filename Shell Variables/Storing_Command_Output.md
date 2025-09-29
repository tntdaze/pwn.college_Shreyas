# Shell Variables

## Storing Command Output
Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!

### Solve
**Flag:** `pwn.college{UXBiB9rTglF38tU_CUJn4KDTNc_.QX1cDN1wiNzAzNzEzW}`

In this challenge, I stored ```/challenge/run``` into PWN variable and used echo on PWN using ```$``` and got the flag.

```bash
PWN=$(/challenge/run)
echo "$PWN"
```

### New Learnings
Learned about storing command output.
