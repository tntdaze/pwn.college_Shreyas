# Processes and Jobs

## Foregrounding Processes
Imagine that you have a backgrounded process, and you want to mess with it some more. What do you do? Well, you can foreground a backgrounded process with fg just like you foreground a suspended process! This level will walk you through that!

### Solve
**Flag:** `pwn.college{0GUlgMDp1wPgDJblbBkv92NLnSk.QX4QDO0wiNzAzNzEzW}`

In this challenge, I ran ```/challenge/run``` then hit ctrl+z and used the ```bg``` command and typed ```fg``` next which printed the flag.

```bash
/challenge/run
ctrl+z
bg
fg
```

### New Learnings
Learned about foregrounding processes.
