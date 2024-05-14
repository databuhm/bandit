## Level 12 -> Level 13

### Level Goal
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

### Solution
`cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'

### Key Concept
'ROT13'
