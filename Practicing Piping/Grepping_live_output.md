# Practicing Piping

## Grepping live output
Now try it for yourself! /challenge/run will output a hundred thousand lines of text, including the flag. grep for the flag!

### Solve
**Flag:** `pwn.college{ARxt-_R5GOpoWorLDlEAGeXsgv9.QX5EDO0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```|``` along with grep and the string ```pwn.college``` which printed the flag. 

```bash
/challenge/run | grep pwn.college
```

### New Learnings
Learned about grepping output.
