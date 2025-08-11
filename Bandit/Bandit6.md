## Goal
---
find the password which is stored somewhere on the server with the following properties:
owned by user bandit7
ownder by a group called bandit6
is 33 bytes in size
## Plan
---
`find / -group bandit6 -user bandit7 -size 33c -type f 2>dev/null`

## Walk Through
---
I start off by researching `ls` options to see if i can filter with groups and/or users. 
I realise `ls` won't help me much so I look into `grep` and `find`.
I find the `-group [gname]`, `-user [uname]`, and `-size [size][size format]`, `-type [type]` for `find`.
I use the command `find / -group bandit6 -user bandit7 -size 33c -type f` and get a lot of `Permission denied`, so I look to outputting to `dev/null` to void all the errors.
I researched to remember how to `STOut` to `dev/null`, and add `2>dev/null` to the command.
I find my file and `cat` it
