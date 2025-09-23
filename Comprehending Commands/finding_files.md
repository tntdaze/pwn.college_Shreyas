# Comprehending Commands

## finding files
Now it's your turn. I've hidden the flag in a random directory on the filesystem. It's still called flag. Go find it!

Several notes. First, there are other files named flag on the filesystem. Don't panic if the first one you try doesn't have the actual flag in it. Second, there're plenty of places in the filesystem that are not accessible to a normal user. These will cause find to generate errors, but you can ignore those; we won't hide the flag there! Finally, find can take a while; be patient!

### Solve
**Flag:** `pwn.college{sIfECs1IL84dAlRE5l7g2gi1wJH.QXyMDO0wiNzAzNzEzW}`

In this challenge, I used find command with name argument as flag which listed all files having flag in its name along with if permission is denied or not. Under this, there was a list of directories:

```bash
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
/opt/linux/linux-5.4/net/mpls/flag
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
/nix/store/7ns27apnvn4qj4q5c82x0z1lzixrz47p-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/5z3sjp9r463i3siif58hq5wj5jmy5m98-python3.12-pwntools-4.13.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/5n5lp1m8gilgrsriv1f2z0jdjk50ypcn-rizin-0.7.3/share/rizin/flag
/nix/store/bnlabj2vsbljhp597ir29l51nrqhm89w-rizin-0.7.4/share/rizin/flag
/nix/store/s8b49lb0pqwvw0c6kgjbxdwxcv2bp0x4-radare2-5.9.8/share/radare2/5.9.8/flag
/nix/store/1hyxipvwpdpcxw90l5pq1nvd6s6jdi5m-python3.12-pwntools-4.14.1/lib/python3.12/site-packages/pwnlib/flag
/nix/store/h88mxp2mbgyj06vypwmqpy05idhwimnp-python3.13-pwntools-4.14.1/lib/python3.13/site-packages/pwnlib/flag
/nix/store/5qz6hgb1qzpvjrsw20wyiylx5zw8b9bk-pwntools-4.14.0/lib/python3.13/site-packages/pwnlib/flag
```
One by one I used ```ls -a``` command on each directory to see if it had a file named flag in it and if it did then I used ```grep pwn.college``` to check if it had the flag. Upon doing this in the second directory it returned the directory name itself so I used the grep command on it and got the flag.

```bash
find / -name flag
ls -a /opt/linux/linux-5.4/net/mpls/flag
grep pwn.college /opt/linux/linux-5.4/net/mpls/flag
```

### New Learnings
Learned about finding files using a specific name as argument.
