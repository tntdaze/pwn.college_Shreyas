# Comprehending Commands

## removing files
This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag!

### Solve
**Flag:** `pwn.college{07dbigXFIYD8T7mEbTq-nV1JRkw.QX2kDM1wiNzAzNzEzW}`

In this challenge, I used ls command to see which files needs to be deleted and ran ```rm delete_me``` to remove it and used ran the check command to get the flag.

```bash
ls
rm delete_me
/challenge/check
```

### New Learnings
Learned about removing files using rm command.
