# Perceiving Permissions

## Groups and Files
In this level, I have made the flag readable by whatever group owns it, but this group is currently root. Luckily, I have also made it possible for you to invoke chgrp as the hacker user! Change the group ownership of the flag file, and read the flag!

### Solve
**Flag:** `pwn.college{cYt7CmEV8_YbRGKE7Ik_w2xrU5Z.QXxcjM1wiNzAzNzEzW}`

In this challenge, I used ```chgrp``` to change the group ownership of the flag file to hacker after which I used ```cat``` on it to get the flag.

```bash
chgrp hacker /flag
cat /flag
```

### New Learnings
Learned about changing groups and files ownerships.
