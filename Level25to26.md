# Level 25 -> Level 26

### Level Goal
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

### Solution
`cat /etc/passwd | grep bandit26`

more trick
1. `ssh -i bandit26.sshkey bandit26@localhost -p 2220` using mini window size terminal
2. `v`
3. `:set shell=/bin/bash`
4. `:sh`
5. `cat /etc/bandit_pass/bandit26`  
