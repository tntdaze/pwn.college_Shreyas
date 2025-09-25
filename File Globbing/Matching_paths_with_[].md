# File Globbing

## Matching paths with []
Once more, we've placed a bunch of files in /challenge/files. Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files!

### Solve
**Flag:** `pwn.college{sJyUE0KBQiqR_r8m-XzR2DBPZUG.QX0IDO0wiNzAzNzEzW}`

In this challenge, I used ```/challenge/run``` command with path of the files that required and their first characters using ```/challenge/files/file_[bash]``` to get the flag.

```bash
/challenge/run /challenge/files/file_[bash]
```

### New Learnings
Learned about matching file paths with [].
