# Level 29 -> Level 30

### Level Goal
There is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

### Solution
1. `mkdir -p /tmp/databuhm29 && cd /tmp/databuhm29`
2. `git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo`
3. `git branch -a`
4. `git checkout {}`
