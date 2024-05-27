# Level 31 -> Level 32

### Level Goal
There is a git repository at ssh://bandit31-git@localhost/home/bandit31-git/repo via the port 2220. The password for the user bandit31-git is the same as for the user bandit31.

Clone the repository and find the password for the next level.

### Solution
1. `mkdir -p /tmp/databuhm31 && cd /tmp/databuhm31`
2. `git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo`
3. `vi key.txt`
4. `git add -f key.txt` #.gitignore
5. `git commit -m "add key.txt"`
6. `git push -u origin master`
