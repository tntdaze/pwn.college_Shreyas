# Pondering Paths

## Position thy self
This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program.

### Solve
**Flag:** `pwn.college{kVoO8urEkuKzu1JWof96aQzWKTy.QX2QTN0wiNzAzNzEzW}`

In this challenge, Firstly, I ran the ```/challenge/run``` command to know which path the flag is in. Then, I used ```cd /etc``` to switch current working directory and ran the challenge command again to get the flag. 

```bash
/challenge/run
cd /etc
/challenge/run
```

### New Learnings
Learned how to change directory and invoking absolute paths from there.
