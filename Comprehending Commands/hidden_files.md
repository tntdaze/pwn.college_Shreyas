# Comprehending Commands

## hidden files
Go find the flag, hidden as a dot-prepended file in /.

### Solve
**Flag:** `pwn.college{Uo9xKURgBwxa44cdp7rrzz2RFrP.QXwUDO0wiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```/``` first then used ```ls -a``` to list all files which listed many files along with 2 dot-prepended files which were ```.dockerenv .flag-229502183726447```. Then, I used cat command on the flag file to get the flag.

```bash
cd /
ls -a
cat .flag-229502183726447
```

### New Learnings
Learned about reading and accessing hidden files using -a command.
