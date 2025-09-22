# Pondering Paths

## The Root
You can invoke a program by providing its path on the command line. In this case, you'll be giving the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path".

### Solve
**Flag:** `pwn.college{oY2_xmsN6DclRauxb4rIbLnBOGd.QX4cTO0wiNzAzNzEzW}`

In this challenge, I invoked pwn command using its absolute path from ```/``` to get the flag.

```bash
/pwn
```

### New Learnings
Learned how to invoke commands using its root.
