# Comprehending Commands

## linking files
In this level the flag is, as always, in /flag, but /challenge/catflag will instead read out /home/hacker/not-the-flag. Use the symlink, and fool it into giving you the flag!

### Solve
**Flag:** `pwn.college{MRLhqhCDk2sjc4IfPBM2jayTZml.QX5ETN1wiNzAzNzEzW}`

In this challenge, firstly I tried reading ```/challenge/catflag``` using cat command which gave the output:
```bash
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
```
Then, I used rm command to remove the ```not-the-flag``` file after which I copied the contents of ```/flag``` which contains the real flag, into a new file with the same name as ```~/not-the-flag``` using ```ln -s``` command. This still gave the same output when I tried reading catflag file. I did the same steps again but this time I renamed the new file to ```home/hacker/not-the-flag``` and got the flag.

```bash
ls /challenge
cat /challenge/catflag
rm not-the-flag
ln -s /flag /home/hacker/not-the-flag
cat /challenge/catflag
```

### New Learnings
Learned about linking and its two types hard and symbolic link.
