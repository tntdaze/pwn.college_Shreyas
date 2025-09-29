# Perceiving Permissions

## Changing Permissions
In this challenge, you must change the permissions of the /flag file to read it! Typically, you need to have write access to the file in order to change its permissions.

### Solve
**Flag:** `pwn.college{oD_tNeDCoBP3DM5WjXMQTQKopdV.QXzcjM1wiNzAzNzEzW}`

In this challenge, I used ```chmod``` with the mode ```o+r``` since it gives read permissions to other users. After this, using ```cat``` on the file printed the flag.

```bash
chmod o+r /flag
cat /flag
```

### New Learnings
Learned about changing file permissions.
