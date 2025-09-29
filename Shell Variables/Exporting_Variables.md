# Shell Variables

## Exporting Variables
In this challenge, you must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported (e.g., not inherited by /challenge/run). Good luck!

### Solve
**Flag:** `pwn.college{0bNFoS3VnBsTGt9LCcsiN0wMT5J.QXyYTN0wiNzAzNzEzW}`

In this challenge, I used ```export``` and set COLLEGE to PWN and set PWN to COLLEGE without export and invoked ```/challenge/run``` and got the flag.

```bash
export PWN=COLLEGE
COLLEGE=PWN
/challenge/run
```

### New Learnings
Learned about exporting variables.
