# Perceiving Permissions

## Fun With Groups Names
The point is, you've used hacker for the group before, but in this level, that is not going to work. I'll still allow you to use chgrp, but I have randomized the name of the group that your user is in. You will need to use the id command to figure that name out, then chgrp to victory!

### Solve
**Flag:** `pwn.college{sPwz1ruIoUwess-k6w-36d1DpZq.QXycjM1wiNzAzNzEzW}`

In this challenge, I ```id``` to check which group hacker user is part of and I found it to be ```grp13741``` and I used ```chgrp``` to change group ownership of flag file to this user and used ```cat``` to get the flag.

```bash
id
chgrp grp13741 /flag
cat /flag
```

### New Learnings
Learned about changing groups and files ownerships.
