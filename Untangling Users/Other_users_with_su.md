# Untangling Users

## Other users with su
In this level, you must switch to the zardus user and then run /challenge/run. Zardus' password is dont-hack-me. Good luck!

### Solve
**Flag:** `pwn.college{EzfrXt9h5WbUYctuFhY9dP_69rv.QX2UDN1wiNzAzNzEzW}`

In this challenge, I used ```su zardus``` to switch to zardus user and typed the given password and typed ```/challenge/run``` to get the flag.

```bash
su zardus
dont-hack-me
/challenge/run
```

### New Learnings
Learned about switching users with su.
