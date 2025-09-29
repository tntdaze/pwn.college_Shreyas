# Data Manipulation

## Extracting specific sections of text
In this challenge, the /challenge/run program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use cut to extract the flag characters, then pipe them to tr -d "\n" (like the previous level!) to join them together into a single line. Your solution will look something like /challenge/run | cut ??? | tr ???, with the ??? filled out.

### Solve
**Flag:** `pwn.college{4fyYXMjkcHs_-tr2_OHI56WNQyn.01NxEzNxwiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` with ```cut -d " " -f 2``` since the flag was in the 2nd column of the text file and used ```tr -d "\n"``` to remove newlines and got the flag.

```bash
/challenge/run | cut -d " " -f 2 | tr -d "\n"
```

### New Learnings
Learned about extracting specific columns of text.
