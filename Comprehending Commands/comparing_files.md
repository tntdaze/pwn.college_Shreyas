# Comprehending Commands

## comparing files
Now for your challenge! There are two files in /challenge:

/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!

### Solve
**Flag:** `> pwn.college{4xBNBAHP1QF8q5xIGzz6O3BUcUL.01MwMDOxwiNzAzNzEzW}`

In this challenge, I used diff command and gave both files as arguments. The terminal printed ```25a26``` and returned the flag after that.

```bash
diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt 
```

### New Learnings
Learned about diff command and how it can be used to compare two files line by line.
