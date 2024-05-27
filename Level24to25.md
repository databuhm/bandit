# Level 24 -> Level 25

### Level Goal
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time

### Solution
`Brute Force`
1. `mkdir -p /tmp/bandit24_databuhm && cd /tmp/bandit24_databuhm`
2. ```
   for i in {0000..9999}
   do
   echo "{bandit24_password} $i"
   done
   ```
3. `./test.sh | nc localhost 30002 | grep -v "Wrong"`
