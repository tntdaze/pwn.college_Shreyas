# Untangling Users

## Cracking passwords
This level simulates this story, giving you a leak of /etc/shadow (in /challenge/shadow-leak). Crack it (this could take a few minutes), su to zardus, and run /challenge/run to get the flag!

### Solve
**Flag:** `pwn.college{I4QCMXssxjIyo-IrNooOYsjwtiO.QX3UDN1wiNzAzNzEzW}`

In this challenge, I used ```john``` command on the given directory of shadow-leak and gave the cracked password as ```aardvark``` and I used su command to switch to zardus user and typed in the password and ran the challenge command and got the flag.

```bash
john /challenge/shadow-leak
su zardus
aardvark
/challenge/run
```

### New Learnings
Learned about cracking passwords using John the Ripper.
