# Level 16 -> Level 17

### Level Goal
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

### Solution
1. `nmap -p 31000-32000 localhost` or `nc -nv -w 1 -z 127.0.0.1 31000-32000 2>&1 | grep succeeded`
2. There are five ports.
3. `openssl s_client -connect localhost:PORT`
4. You will get RSA PRIVATE KEY.
5. `mktemp -d`
6. `vi sshkey`
7. `chmod 600 sshkey`
8. `ssh -i sshkey bandit17@localhost -p 2220`
