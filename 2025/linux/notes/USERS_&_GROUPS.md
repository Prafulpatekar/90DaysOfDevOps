
1. **Get current username** - To check what user is logged in. Session User
```sh
whoami
```

2. **list of all users** - To check all users on server.
```sh
cat /etc/passwd
```

3. **Create New user** - To create or add new user. -m (make a home dir folder) to give folder and this command needs sudo permissions. -s to give shell to user. This command will create group as well for the user by default.
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

4. **Create password for user** - To create new password for user. Enter the command and prompt will ask to enter new password.
```sh
sudo passwd <username>
```

5. **Switch user** - To switch user.
```sh
su <username>
```

6. **Delete user** - To delete user.
```sh
sudo userdel <username>
```

7. **List of all groups** - To check all groups on server.
```sh
cat /etc/group
```

8. **Create group** - To create only group. when you want to create only group but not user.
```sh
sudo groupadd <groupname> 
```

9. **Add users to group** - To add multiple users to group via username. -M stands for multiple args
```sh
sudo gpasswd -M <username1>,<username2> <groupname>
```

10. **Add User via usermod command** - To add user using user modification command. -a stands for append and G is for group.
```sh
sudo usermod -aG <groupname> <username>
```

11. **Delete user from a group** - To delete any user from a group.
```sh
sudo gpasswd -d <username> <groupname>
```

12. **Change Owner** - To change ownership of any file/folder.
```sh
sudo chown <username> /path/to/file_or_folder
```

13. **Change Group** -  To change ownership of any file/folder.
```sh
sudo chgrp <groupname> /path/to/file_or_folder
``` 