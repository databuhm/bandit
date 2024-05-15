# Level 12 -> Level 13

### Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed.
For this level it may be useful to create a directory under /tmp in which you can work.
Use mkdir with a hard to guess directory name.
Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

### Solution
1. `mktemp -d`
2. /tmp/tmp.cU4dx3PTPO
3. `cp data.txt /tmp/tmp.cU4dx3PTPO`
4. `xxd -r data.txt > bandit`
5. `gunzip {filename.gz}`
6. `bzip2 -d {filename.bz2}`
7. `tar -xf {filename.tar}`

### Key Concept
`Repeatedly and in various methods, compressed files`
