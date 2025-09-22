# Pondering Paths

## implicit relative paths, from /
You'll need to run /challenge/run using a relative path while having a current working directory of /.

### Solve
**Flag:** `pwn.college{osZ-2uT1GtUv16s8lgK_yKY6AP2.QX5QTN0wiNzAzNzEzW}`

In this challenge, I used cd command to change directory to / and then ran ```challenge/run``` command to get the flag.

```bash
cd /
challenge/run
```

### New Learnings
Learned how to invoke commands using implicit relative paths.
