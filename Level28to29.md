# Level 28 to Level 29

### Level Goal
There is a git repository at ssh://bandit28-git@localhost/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28.

Clone the repository and find the password for the next level.

### Solution
1. `mkdir -p /tmp/databuhm28 && cd /tmp/databuhm28`
2. `git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo`
3. `git log`
4. `git checkout {}`
