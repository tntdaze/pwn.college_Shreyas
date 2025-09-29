# Data Manipulation

## Sorting data
In this challenge, there's a file at /challenge/flags.txt containing 100 fake flags, with the real flag mixed among them. When sorted alphabetically, the real flag will be at the end (we made sure of this when generating fake flags). Go get it!

### Solve
**Flag:** `pwn.college{kJAfYeWfnfF3LSb0uSPiexjrP6-.0FM0MDOxwiNzAzNzEzW}`

In this challenge, I used ```sort``` on the given file and used ```-r``` to print it in reverse since the flag is at the end.

```bash
sort /challenge/flags.txt -r
```

### New Learnings
Learned about sorting data.
