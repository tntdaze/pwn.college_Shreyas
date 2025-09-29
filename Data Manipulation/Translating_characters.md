# Data Manipulation

## Translating characters
In this level, /challenge/run will print the flag but will swap the casing of all characters (e.g., A will become a and vice-versa). Can you undo it with tr and get the flag?

### Solve
**Flag:** `pwn.college{ES-oqERLxyFariN-seprol_GxtN.01MxEzNxwiNzAzNzEzW}`

In this challenge, I first tried using ```tr``` to swap ABC... and so on with abc... which didn't work so I tried the opposite of this. Then, I realized that uppercase needs to be made lowercase and vice verca so I tried ```tr a-zA-Z A-Za-z``` which worked and I got the proper cased flag.

```bash
/challenge/run | tr a-zA-Z A-Za-z
```

### New Learnings
Learned about translating characters.
