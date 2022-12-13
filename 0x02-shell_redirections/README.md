0. echo "Hello, World" prints “Hello, World”, followed by a new line to the standard output.
1. echo -e '"(Ôo)'\' displays a confused smiley "(Ôo)'.
2. cat /etc/passwd displays the content of the /etc/passwd file.
3. cat /etc/passwd /etc/hosts displays the content of /etc/passwd and /etc/hosts.
4. l -n 10 /etc/passwd displays the last 10 lines of /etc/passwd.
5. head -n 10 /etc/passwd displays the first 10 lines of /etc/passwd.
6. head -n 3 iacta | tail -n 1 displays the third line of the file iacta.
7. echo "Best School" > "\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)" creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
8. ls -la>ls_cwd_content writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
9. tail -n 1 iacta >> iacta duplicates the last line of the file iacta.
10. find . -type f -name "*.js" -delete deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
11. find ./* -type d | wc -l counts the number of directories and sub-directories in the current directory.
12. ls -t -1 | head displays the 10 newest files in the current directory.
13. sort | uniq -u takes a list of words as input and prints only words that appear exactly once.
14. grep -e "root" /etc/passwd displays lines containing the pattern “root” from the file /etc/passwd.
15. grep -c "bin" /etc/passwd displays the number of lines that contain the pattern “bin” in the file.
16. grep -A 3 "root" /etc/passwd displays lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.
17. grep -v "bin" /etc/passwd displays all the lines in the file /etc/passwd that do not contain the pattern “bin”.
18. grep ^[a-zA-Z] /etc/ssh/sshd_config displays all lines of the file /etc/ssh/sshd_config starting with a letter.
19. tr A Z | tr c e replaces all characters A and c from input to Z and e respectively.
20. tr -d c | tr -d C removes all letters c and C from input.
21. rev reverse the input.
22. cut -d':' -f 1,6 /etc/passwd | sort displays all users and their home directories, sorted by users. Based on the the /etc/passwd file
23. find . -empty -printf "%f\n" finds all empty files and directories in the current directory and all sub-directories.

	-Only the names of the files and directories should be displayed (not the entire path)

	-Hidden files should be listed

	-One file name per line

	-The listing should end with a new line

	-You are not allowed to use basename, grep, egrep, fgrep or rgrep.

24. find -type f -name "*.gif" -printf "%f\n" | rev | cut -d'.' -f 2- | rev | LC_ALL=C sort -f lists all the files with a .gif extension in the current directory and all its sub-directories.

	-Hidden files should be listed.

	-Only regular files (not directories) should be listed.

	-The names of the files should be displayed without their extensions.

	-The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay).

	-One file name per line.

	-The listing should end with a new line.

	-You are not allowed to use basename, grep, egrep, fgrep or rgrep.

25. cut -b 1 | tr -d '\n' | uniq decodes acrostics that use the first letter of each line.

	-The ‘decoded’ message has to end with a new line.

	-You are not allowed to use grep, egrep, fgrep or rgrep.

26. tail -n +2 | cut -f1 | sort | uniq -c | sort -nr | head -11 | tr -s ' ' | cut -d' ' -f3 parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.

	-Order by number of requests, most active host or IP at the top.

	-You are not allowed to use grep, egrep, fgrep or rgrep.
