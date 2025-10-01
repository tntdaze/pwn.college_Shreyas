# Practicing Piping

## Named pipes
This challenge will be a simple introduction to FIFOs. You'll need to create a /tmp/flag_fifo file and redirect the stdout of /challenge/run to it. If you're successful, /challenge/run will write the flag into the FIFO! Go do it!

HINT: The blocking behavior of FIFOs makes it hard to solve this challenge in a single terminal. You may want to use the Desktop or VSCode mode for this challenge so that you can launch two terminals.

### Solve
**Flag:** `pwn.college{4F_IKRxSMp4uY0g4inMVGG6JQ3q.01MzMDOxwiNzAzNzEzW}`

In this challenge, I used ```mkfifo``` and made ```/tmp/flag_fifo``` file and redirected stdout of ```/challenge/run``` to it after which I tried using cat command on it but didn't work. So, after reading the hint they provided I opened another terminal and used cat command over there which printed the flag.

Terminal 1
```bash
mkfifo /tmp/flag_fifo
/challenge/run > /tmp/flag_fifo
```
Terminal 2
```bash
cat /tmp/flag_fifo
```

### New Learnings
Learned about named pipes.
