# Pondering PATH

## Setting PATH
This level's /challenge/run will run the win command via its bare name, but this command exists in the /challenge/more_commands/ directory, which is not initially in the PATH. The win command is the only thing that /challenge/run needs, so you can just overwrite PATH with that one directory. Good luck!

### Solve
**Flag:** `pwn.college{gKNYZ_2CDC09yRBZojxILxxMKz8.QX1cjM1wiNzAzNzEzW}`

In this challenge, I typed ```PATH=/challenge/more_commands``` and used ```/challenge/run``` and got the flag.

```bash
PATH=/challenge/more_commands
/challenge/run
```

### New Learnings
Learned about the setting the PATH variable.
