#Bandit 0
!(https://res.cloudinary.com/s1n1s73r-k1773n/image/upload/v1624315610/overthewire/Bandit0_thh95i.png) 

The file was stored in the home directory readme.
-ls to list file
-cat command to display contents of readme
Bandit 1
 
The file – is located in the home directory, so use ls to display 
Use ./ current directory to display files with – 

Bandit 2
 
List files ls
Use cat with back slashes before spaces so that it doesn’t think there are 4 different files instead of one. 

Bandit 3
 
The password is in a hidden file. 
•	Use ls to display contents, but it doesn’t show. 
•	I used ls -la to display all files, including hidden ones.
•	Used ‘.’ at the beginning, to open the hidden file.
Bandit 4
 
•	All files have a  - and it’s the only human-readable one
•	Used the file cmd  and file* as a wild card 
•	Shows file 7 as the readable 
Bandit 5
 
•	ls to list files in inhere
•	Since there were so many files within the files, I used the  find cmd
•	find cmd shows only one file that has the size given for the password
Bandit 6
 
•	on the server somewhere, so used find cmd
•	displayed too many files so narrowed my search to size, user, and group
•	found the /var/lib/dpkg/info/bandit7.password and displayed content
Bandit 7
 
•	showed many lines of text
•	used pipe to grep to find the word millionth
•	displayed one line, giving us the password

Bandit 8
 
•	need to use pipe and sort 
•	sorted the files and then piped it to uniq to show the unique password
Bandit 9
 
•	the contents of the file is mostly human unreadable text
•	used the strings cmd and grep to look for = signs

Bandit 10
 
•	after displaying contents in the file, a base64 code was given
•	used cyberchef to decode it.
Bandit 11
 
•	The file contained a rot13 code
•	Decrypted with cyber chef


 In this lab, I was only able to complete level 12. I was able to create a directory but wasn’t sure where to go from that point. I used Google to find out what to do when a hexdump file has been repeatedly compressed as well as looking up the other clues given. 
