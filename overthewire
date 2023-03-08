level 0:
	ssh bandit0@bandit.labs.overthewire.org -p 2220
	*password
	bandit0
level 1:
	less ~/readme
	*we logout and login again
	ssh bandit1@bandit.labs.overthewire.org -p 2220
	*password
	NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
level 2:
	cat < -
	*we logout and login again
        ssh bandit2@bandit.labs.overthewire.org -p 2220
	*password
	rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
level 3:
	cat spaces\ in\ this\ filename
	*password
	aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
level 4:
	cd inhere
	ls -a
	cat .hidden
	*password
	2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
level 5:
	cd inhere
	ls -a
	cat < -file00
	cat < -file01
	...
	cat < -file07
	*contains the password
	*password
	lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
level 6:
	*exiting from ssh
	exit
	ssh bandit5@bandit.labs.overthewire.org -p 2220
	lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
	ls -a
	cd inhere
	ls -a
	find -size 1033c -readable ! -executable
	cat ./maybehere07/.file2
	*password
	P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
level 7:
	find / -user bandit7 -group bandit6 -size 33c
	*the above will give us many permission denied errors
	*also we are not allowed to run sudo on a remote pc
	find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
	cat /var/lib/dpkg/info/bandit7.password
	*password
	z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
level 8:
	ls -a
	grep 'millionth' data.txt  /dev/null
	*password
	TESKZC0XvTetK0S9xNwm25STk5iWrBvP
level 9:
	
