# Perceiving Permissions

## The SUID Bit
Now, we are going to let you add the SUID bit to the /challenge/getroot program in order to spawn a root shell for you to cat the flag yourself!

### Solve
**Flag:** `pwn.college{E_Eppx5fEiXzyAPKCjn24tZGiGs.QXzEjN0wiNzAzNzEzW}`

In this challenge, I set the permissions of ```/challenge/getroot``` to ```u=rws``` using ```chmod``` and then entered the root shell where I used cat to get the flag.

```bash
chmod u=rws /challenge/getroot
/challenge/getroot
cat /flag
```

### New Learnings
Learned about SUID bit.
