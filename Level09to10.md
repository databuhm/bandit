# Level 9 -> Level 10

### Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings,
preceded by several ‘=’ characters.

### Solution
`strings data.txt | grep =`
