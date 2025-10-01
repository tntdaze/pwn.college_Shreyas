# Chaining Commands

## Building on Success
In this challenge, you need to chain the programs /challenge/first-success and /challenge/second using the && operator. Try running each command separately first to see what happens (which is that you will not get the flag). But if you chain them with &&, the flag will appear!

### Solve
**Flag:** `pwn.college{ADXnuNUa3j4KccjiFHhScyepEIC.0lM0MDOxwiNzAzNzEzW}`

In this challenge, I ran ```/challenge/first-success``` separated by ```&&``` and ```/challenge/second``` to get the flag.

```bash
/challenge/first-success && /challenge/second
```

### New Learnings
Learned about building on success using &&.
