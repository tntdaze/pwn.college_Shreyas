# Untangling Users

## Becoming root with su
This challenge (and only this challenge) does have a root password. That password is hack-the-planet, and you must provide it to su to become root! Go do that, and read the flag!

### Solve
**Flag:** `pwn.college{437fimUSODUHiymUhaFLto7Yd9z.QX1UDN1wiNzAzNzEzW}`

In this challenge, I used ```su``` and typed the given password and used cat command to get the flag.

```bash
su
hack-the-planet
cat /flag
```

### New Learnings
Learned about root and su command.
