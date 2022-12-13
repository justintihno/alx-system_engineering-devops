1. su betty switches the current user to the user betty.
2. whoami prints the effective username of the current user.
3. groups prints all the groups the current user is part of.
4. sudo chown betty hello changes the owner of the file hello to the user betty.
5. touch hello creates an empty file called hello.
6. chmod u+x hello adds execute permission to the owner of the file hello.
7. chmod +114 hello adds execute permission to the owner and the group owner, and read permission to other users to the file hello.
8. chmod +111 hello adds execute permission to the group owner, the group and the other users to the file hello.
9. chmod 007 hello sets the permission to the file hello as follows.

  -Owner: no permission at all.
  
  -Group: no permission at all.
  
  -Other users: all the permissions.
  
10. chmod 753 hello sets the mode of the file hello as follows:
  
  -rwxr-x-wx
  
11. chmod --reference=olleh hello sets the mode of the file hello the same as olleh's mode.
12. chmod a+x */ adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
13. mkdir -m 751 my_dir creates a directory called my_dir with permissions 751 in the working directory.
14. chgrp school hello changes the group owner to school for the file hello.
15. chown vincent:staff * changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
16. chown -h vincent:staff _hello changes the owner and the group owner of _hello to vincent and staff respectively.
17. chown --from=guillaume betty hello changes the owner of the file hello to betty only if it is owned by the user guillaume.
18. telnet towel.blinkenlights.nl plays the StarWars IV episode in the terminal.
