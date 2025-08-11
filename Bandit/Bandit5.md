## Goal
---
Find the password in the file with the following properties:
- human-readable
- 1033 bytes
- not executable
## Plan
---
`ls -lARS`
`cat [file]`

## Walk Through
---
I `cd inhere` and `ls -l` finding multiple directories. After brute forcing the previous task I do not want to brute force through all the files in the sub-directories. So i do further research on `ls`.
I find the `-R` option for sub-directories, `-h` option for human readable, `-s` for the size.
I use the `ls -lRhs` and went through the outputs not finding the file and looking into a few of the files to see they all look to have readable text. So I look further into the `ls` options.
I find the `-S` option and saw the `-A` reminding me to check for hidden files.
I use my new command `ls -lARS` and find my file
