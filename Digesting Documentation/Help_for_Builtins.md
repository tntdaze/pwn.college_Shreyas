# Digesting Documentation

## Help for Builtins
In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!

### Solve
**Flag:** `pwn.college{47jMmA77kM4AHh3ePIIHx8lvkKY.QX0ETO0wiNzAzNzEzW}`

In this challenge, I used help command on challenge which printed:
```bash
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "47jMmA77".
```
I typed out the secret value with ```challenge --secret``` and got the flag.

```bash
help challenge
challenge --secret 47jMmA77
```

### New Learnings
Learned about builtin help command.
