## Goal
---
Find the password stored in the `data.txt` next to the word millionth
## Plan
---
`cat data.txt | grep "millionth"`

## Walk Through
---
I `ls` to see the file. I know that I will need to use `grep` to parse through the file.
I do research on `grep` to find the password, after a short research I remember that I can use `|` (pipe) to use `grep` to filter `cat`.
I use the command `cat data.txt | grep "millionth"` to test and it worked
