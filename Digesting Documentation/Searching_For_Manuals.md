# Digesting Documentation

## Searching For Manuals
This level is tricky: it hides the manpage for the challenge by randomizing its name. Luckily, all of the manpages are gathered in a searchable database, so you'll be able to search the man page database to find the hidden challenge man page! To figure out how to search for the right manpage, read the man page manpage by doing: man man!

### Solve
**Flag:** `pwn.college{UbtwFYe4kDsuwLvuLjm61inrN04.QX2EDO0wiNzAzNzEzW}`

In this challenge, I used ```man man``` to get the manual for man and saw under examples section that ```man -k {keyword}``` is used for searching manual page names for the specific keyword and used it for challenge and the terminal printed:
```bash
btweksuwvu (1)       - print the flag!
```
Then, I used man command on this which popped up the manual for /challenge/challenge and used ```--btweks NUM``` where NUM is 461 to get the flag.

```bash
man man
man -k challenge
man btweksuwvu
/challenge/challenge --btweks 461
```

### New Learnings
Learned about searching for manuals.
