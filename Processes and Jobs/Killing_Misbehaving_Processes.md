# Processes and Jobs

## Killing Misbehaving Processes
Your general workflow should be:

Check what processes are running.
Find /challenge/decoy in the list and figure out its process ID.
kill it.
Run /challenge/run to get the flag without being overwhelmed by decoys (you don't need to redirect its output; it'll write to the FIFO on its own).
Good luck!

### Solve
**Flag:** `pwn.college{wvrkDuNVNe0LuC4msbIjQgmnGQ5.0FNzMDOxwiNzAzNzEzW}`

In this challenge, I ran ```ps aux``` and saw PID 142 had the decoy and killed it after which I ran ```/challenge/run``` but it got stuck at sending the flag to the fifo file. So, I used cat command first on the flag_fifo file which printed many decoys. Upon reading the NOTE given in the instructions I interrupted the terminal and ran ```/challenge/run``` which printed:
```bash
Sending the flag to /tmp/flag_fifo!
```
Then, I used cat command on the flag_fifo file and got the flag.

```bash
ps aux
kill 142
cat /tmp/flag_fifo
/challenge/run
cat /tmp/flag_fifo
```

### New Learnings
Learned about killing misbehaving processes.
