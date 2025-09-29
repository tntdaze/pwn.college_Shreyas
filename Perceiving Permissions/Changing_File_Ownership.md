# Perceiving Permissions

## Changing File Ownership
In this level, we will practice changing the owner of the /flag file to the hacker user, and then read the flag. For this challenge only, I made it so that you can use chown to your heart's content as the hacker user (again, typically, this requires you to be root). Use this power wisely and chown away!

### Solve
**Flag:** `pwn.college{smwqEPoHMCkpHzdvdatJGjvMgQZ.QXxEjN0wiNzAzNzEzW}`

In this challenge, I used ```chown``` command and changed the ownership of /flag file to hacker and used ```cat``` on it to get the flag.

```bash
chown hacker /flag
cat /flag
```

### New Learnings
Learned about changing file ownerships.
