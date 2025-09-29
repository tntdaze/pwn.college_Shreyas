# Processes and Jobs

## Killing Processes
Now, it's time to terminate your first process! In this challenge, /challenge/run will refuse to run while /challenge/dont_run is running! You must find the dont_run process and kill it. If you fail, pwn.college will disavow all knowledge of your mission. Good luck.

### Solve
**Flag:** `pwn.college{gcc2c3YZKxLU6qyL7fFSNyW_Jm3.QXyQDO0wiNzAzNzEzW}`

In this challenge, I used ```ps -e | grep /challenge/dont_run``` which didn't print anything or do anything so I tried ```ps -e | grep dont_run``` which didn't do anything again then I tried doing what was given in the instruction's example so I used sleep with grep which gave me the PID and I used ```kill 137``` and ran the file which printed the file.

```bash
ps -e | grep sleep
kill 137
/challenge/run
```

### New Learnings
Learned about killing processes.
