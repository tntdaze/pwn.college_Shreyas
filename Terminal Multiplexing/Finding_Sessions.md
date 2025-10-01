# Terminal Multiplexing

## Finding Sessions
In this challenge, we've created three screen sessions for you. One of them contains the flag. The other two are decoys!

### Solve
**Flag:** `pwn.college{gv6UsKZ3nf6q_WlplNc7pjx4WwR.01N4IDOxwiNzAzNzEzW}`

In this challenge, I used ```screen -ls``` to list out all current screens and attached each one by one until I found the right session with the flag.

```bash
screen -ls
screen -r {session}
```

### New Learnings
Learned how to find sessions.
