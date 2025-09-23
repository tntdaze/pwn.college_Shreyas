# Comprehending Commands

## making directories
Now, go forth and create a /tmp/pwn directory and make a college file in it! Then run /challenge/run, which will check your solution and give you the flag!

### Solve
**Flag:** `pwn.college{YdcdtPHylrrl6FBYiQArlyCvuWO.QXxMDO0wiNzAzNzEzW}`

In this challenge, I used mkdir command twice to make ```tmp``` and ```pwn``` and changed directory to ```/tmp/pwn``` after which I used touch command to create the file ```college``` and got the flag.

```bash
mkdir tmp
cd /tmp
mkdir pwn
cd /tmp/pwn
touch college
/challenge/run
```

### New Learnings
Learned about making directories using mkdir command.
