# Comprehending Commands

## An Epic Filesystem Quest
In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it! Here's how it'll work:

Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!

### Solve
**Flag:** `pwn.college{EWm5G0Js4wx6n1y7CiZdVfSD641.QX5IDO0wiNzAzNzEzW}`

In this challenge, I used cd to change directory to ```/``` first then used ```ls``` to list all files which listed many files and I used cat command to read the ```SNIPPET``` file and it kept redirecting me to different directories and files which had either trapped or delayed files so accordingly I followed it to get the flag at last. 

```bash
cd /
ls
cat SNIPPET
cd /usr/share/zsh/help
ls -a
cat .GIST
ls -a /opt/linux/linux-5.4/arch/h8300/include
cat /opt/linux/linux-5.4/arch/h8300/include/TRACE-TRAPPED
cd /usr/lib/python3/dist-packages/networkx/algorithms/centrality/tests/__pycache__
ls
cat DIPATCH
cd /opt/kropr/target/release/build/thiserror-aea5e1d8f1f0e842
ls
cat README
ls -a /opt/linux/linux-5.4/arch/s390/kernel/
cat /opt/linux/linux-5.4/arch/s390/kernel/TIP-TRAPPED
cd /opt/linux/linux-5.4/drivers/net/ethernet/amd
ls
cat EVIDENCE
ls -a /usr/lib/ruby/2.7.0/bundler/source/git
cd /usr/lib/ruby/gems/2.7.0/gems/observer-0.1.0
ls -a
cat NOTE
```

### New Learnings
Learned how I can follow around clues or hints to eventually get the flag.
