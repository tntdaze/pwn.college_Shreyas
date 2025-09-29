# Practicing Piping

## Filtering with grep -v
Sometimes, the only way to filter to just the data you want is to filter out the data you don't want. In this challenge, /challenge/run will output the flag to stdout, but it will also output over 1000 decoy flags (containing the word DECOY somewhere in the flag) mixed in with the real flag. You'll need to filter out the decoys while keeping the real flag!

### Solve
**Flag:** `pwn.college{8PptcfoyLecPXZYbxJ4vk5Kb58-.0FOxEzNxwiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with grep using ```|``` operator and filtered it so that there's no DECOY in the name and got the flag.

```bash
/challenge/run | grep -v DECOY
```

### New Learnings
Learned about filtering with grep using -v.
