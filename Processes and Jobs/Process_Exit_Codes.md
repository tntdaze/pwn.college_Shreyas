# Processes and Jobs

## Process Exit Codes
In this challenge, you must retrieve the exit code returned by /challenge/get-code and then run /challenge/submit-code with that error code as an argument. Good luck!

### Solve
**Flag:** `pwn.college{8cgtWg0M8OLeAn7jsfP_jlXq8AH.QX5YDO1wiNzAzNzEzW}`

In this challenge, I ran ```/challenge/get-code``` and used ```echo $?``` as given in the instructions and got the error code as ```57``` then used it as argument with ```/challenge/submit-code```

```bash
/challenge/get-code
echo $?
/challenge/submit-code 57
```

### New Learnings
Learned about exit codes.
