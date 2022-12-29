0x00. Shell, basics


0-current_working_directory - prints the absolute path name of the current working directory

1-listit - display the contents list of your current directory

2-bring_me_home - changes the working directory to the user’s home directory

3-listfiles - displays current directory contents, including hidden files (starting with .). Use the long format

4-listmorefiles - Display current directory contents:
    - Long format
    - With user and group IDs displayed numerically
    - And hidden files (starting with .)

5-listfilesdigitonly -  creates a directory named folder in the /tmp/ directory

6-firstdirectory - moves the file betty from /tmp/ to /tmp/folder

7-movethatfile - deletes the file betty. The file betty is in /tmp/folder

8-firstdelete - deletes the directory folder that is in the /tmp directory

9-firstdirdeletion - changes the working directory to the previous one

10-back - lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format

11-lists - lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format

12-file_type - prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script

13-symbolic_link - a symbolic link to /bin/ls, named ls. The symbolic link should be created in the current working directory

14-copy_html - a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory

100-lets_move - moves all files beginning with an uppercase letter to the directory /tmp/u

101-clean_emacs - a script that deletes all files in the current working directory that end with the character ~

102-tree - a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory

103-commas - a command that lists all the files and directories of the current directory, separated by commas (,).
    - Directory names should end with a slash (/)
    - Files and directories starting with a dot (.) should be listed
    - The listing should be alpha ordered, except for the directories . and .. which should be listed at the very beginning
    - Only digits and letters are used to sort; Digits should come first
    - You can assume that all the files we will test with will have at least one letter or one digit
    - The listing should end with a new line

school.mgc - a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0.