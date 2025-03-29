# LINUX Day To Day Commands as Devops Engineer

1. **grep** - Global Regular Expression Print
```sh
grep -i "authentication file" app_log.txt | head -n 5
```
OR
```sh
grep -i "authentication file" app_log.txt | tail -n 5
```

2. **awk** - Named after its creators Aho, Weinberger, and Kernighan
Simple Print file as is
```sh
awk '{print}' app_log.txt 
```
To add a regex patter search
```sh
awk '/authentication failure/ {print}' app_log.txt
```
To selected columns e.g. $1 and $2 are columns.
```sh
awk '/authentication failure/ {print $1, $2}' app_log.txt
```
To filter via and column e.g. Date and Month
```sh
awk '/authentication failure/ {if ($1=="Jul" && $2=="26") print $13, $14}' app_log.txt
```

3. **sed** - File Stream Editor to edit file stream
To replace string 'user' with 'username'
```sh
sed "s/user/username/g" auth_fail_logs.txt 
```
for multiple args 
```sh
sed "s/user/username/g; s/rhost/IP/g" auth_fail_logs.txt
```
For unique results
```sh
sed "s/user/username/g; s/rhost/IP/g" auth_fail_logs.txt | uniq
```

4. **find** - To find any file or dir in linux  server. 
```sh
find <dir/path/where/needs/to/find> -name <filename>
```