# Comprehending Commands

## touching files
In this level, please create two files: /tmp/pwn and /tmp/college, and run /challenge/run to get your flag!

### Solve
**Flag:** `pwn.college{URCOfgdQn4CKdysP_ifxyOkJmLh.QXwMDO0wiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```tmp``` and then used touch command twice to create the two files needed and ran ```/challenge/run``` to get the flag.

```bash
cd /tmp
touch pwn
touch college
/challenge/run
```

### New Learnings
Learned about creating new files using touch command.
