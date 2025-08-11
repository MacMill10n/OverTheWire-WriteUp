## Goal
---
Find the password in the `data.txt` in the line of text that occurs only once
## Plan
---
`sort data.txt | uniq -u`

## Walk Through
---
I presume i will need to use `grep` and `|` again, so I do some research into how I can use `grep` to find a unique line.
I don't find anything useful, so I do general research on how to find unique lines in a text file and find `sort [file] | uniq -u`. 
I works so I make a note to look into `sort` and `uniq`.
