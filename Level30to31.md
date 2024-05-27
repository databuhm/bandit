# Level 30 -> Level 31

### Level Goal
There is a git repository at ssh://bandit30-git@localhost/home/bandit30-git/repo via the port 2220. The password for the user bandit30-git is the same as for the user bandit30.

### Solution
1. `mkdir -p /tmp/databuhm30 && cd /tmp/databuhm30`
2. `git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo`
3. `git tag`
4. `git show {}`
