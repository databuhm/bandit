# Level 20 -> Level 21

### Level Goal
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

### Solution
1. Log in as the bandit20 user in the terminal and start the first session.
2. Open a new terminal, log in as the bandit20 user again, and start the second session.
3. `nc -lnvp 7777` in the second session.
4. `./suconnect 7777` in the first session.
5. Enter the password for bandit20 in the second session.
