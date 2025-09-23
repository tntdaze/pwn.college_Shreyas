# Comprehending Commands

## listing files
In this challenge, we've named /challenge/run with some random name! List the files in /challenge to find it.

### Solve
**Flag:** `pwn.college{IGv11fPCzTGxhd-tYAutENUj163.QX4IDO0wiNzAzNzEzW}`

In this challenge, first I ran ```ls /challenge``` command to see which file is renamed. Then it gave 2 file name as outputs ```4326-renamed-run-31422  DESCRIPTION.md``` and I tried using cat command in the renamed-run file which gave the output:
```bash
#!/opt/pwn.college/bash

echo "Yahaha, you found me! Here is your flag:"
cat /flag
```
I typed ```cat /flag``` command which gave permission denied error and then I typed in the file directory which gave the flag.

```bash
ls /challenge
cat /challenge/4326-renamed-run-31422
/challenge/4326-renamed-run-31422
```

### New Learnings
Learned about using ls command and how it works.
