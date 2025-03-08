# List of commands in linux

1. **echo** - To print variables or strings on screen,  basically anything
```sh
echo "hello world!"
```

2. **mkdir** - To create a directory of given name
```sh
mkdir devops
```

3. **cd** - To change directory
```sh
cd devops
```

4. **touch** - To create a file of given name with extension
```sh
touch my_file.txt
```

5. **ls** - To list all files and directories of current directory. grep search the patterns in files and folders
```sh
ls
```
or
```sh
ls | grep ".txt"
```


6. **pwd** - To know present current directory
```sh
pwd
```

7. **man** - To know about any command
```sh
man ls
```

8. **rm** - To remove/delete files 
```sh
rm my_file.txt
```

9. **rm -rm** - To forcefully remove/delete files/dirs 
```sh
rm -rf demo/
```

10. **rm -rm** - To forcefully remove/delete files/dirs 
```sh
rm -rf demo/
```

11. **sudo** - It is group with all permissions and privileges. You required this when you are trying run any command that needs superuser/root user permissions.
```sh
sudo apt-get install nginx
```

12. **systemctl** - It is tool/service for control manager. (It's like ctrl+alt+del in windows). You can start/stop/enable or check status of any service
```sh
systemctl status nginx
```
```sh
sudo systemctl stop nginx
```
```sh
sudo systemctl start nginx
```
```sh
sudo systemctl enable nginx
```

13. **whoami** - To check what user is logged in. Session User
```sh
whoami
```

14. **cat /etc/passwd** - To check all users on server.
```sh
cat /etc/passwd
```

15. **Create New user** - To create or add new user. -m (make a home dir folder) to give folder and this command needs sudo permissions. -s to give shell to user.
```sh
sudo useradd -m <username>
```
or
```sh
sudo useradd <username>
```
or 
```sh
sudo useradd -m <username> -s /bin/bash
```

16. **Create password for user** - To create new password for user. Enter the command and prompt will ask to enter new password.
```sh
sudo passwd <username>
```

17. **Switch user** - To swtich user.
```sh
su <username>
```

18. **View Running processes** - To view running process
```sh
ps
```

19. **view disk space usage** - To view disk space usage in linux.
```sh
df -h
```

20. **terminate a process** - To terminate a process in linux.
```sh
kill
```