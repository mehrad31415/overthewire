# should you want to replace a certain word or element in a file:
# sed 's/\*/#/g' old_file_name | cat > new_file_name
# or you can do it inplace using the -i option of sed and there is no need for piping.
# sed (like awk and tr) are related scripting languages to bash.

level 0:
	ssh bandit0@bandit.labs.overthewire.org -p 2220
	#enter the password (bandit0)
	#exiting from ssh is with the exit command.
level 1:
	#do not log out from bandit0 (if logged out, repeat level0).
	less readme
	#the password in the file is:
	NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
level 2:
	ssh bandit1@bandit.labs.overthewire.org -p 2220
	#enter the password (NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL)
	cat < -
	#the password in the file is:
	rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi
level 3:
	ssh bandit2@bandit.labs.overthewire.org -p 2220
	#enter the password (rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi)
	cat 'spaces in this filename' (or cat spaces\ in\ this\ filename)
	#the password in the file is:
	aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
level 4:
	ssh bandit3@bandit.labs.overthewire.org -p 2220
	#enter the password (aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG)
	cd inhere
	ls -a
	cat .hidden
	#the password in the file is:
	2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe
level 5:
	ssh bandit4@bandit.labs.overthewire.org -p 2220
	#enter the password (2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe)
	cd inhere
	ls -a
	cat < -file00
	cat < -file01
	...
	cat < -file07
	#contains the password
	#the password in the file is:
	lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
level 6:
	ssh bandit5@bandit.labs.overthewire.org -p 2220
	#enter the password (lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR)
	find -readable ! -executable -size 1033c
	cat ./inhere/maybehere07/.file2
	#the password in the file is:
	P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
level 7:
	ssh bandit6@bandit.labs.overthewire.org -p 2220
	#enter the password (P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU)
	find / -user bandit7 -group bandit6 -size 33c
	#the above will give us many permission denied errors
	#also we are not allowed to run sudo on a remote pc
	#2>/dev/null means redirect all the error message to /dev/null and only show the 'valid' msgs
	#using cat in the piping below will only give the name of the file back.
	find / -user bandit7 -group bandit6 -size 33c 2>/dev/null | xargs cat
	#the password in the file is:
	z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
level 8:
	ssh bandit7@bandit.labs.overthewire.org -p 2220
	#enter the password (z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S)
	ls -a
	grep 'millionth' data.txt
	#the password in the file is:
	TESKZC0XvTetK0S9xNwm25STk5iWrBvP
level 9:
	ssh bandit8@bandit.labs.overthewire.org -p 2220
	#enter the password (TESKZC0XvTetK0S9xNwm25STk5iWrBvP)
	sort --ignore-case data.txt | uniq -u
	#the password in the file is:
	EN632PlfYiZbn3PhVK3XOGSlNInNE00t
level 10:
	ssh bandit9@bandit.labs.overthewire.org -p 2220
	#enter the password (EN632PlfYiZbn3PhVK3XOGSlNInNE00t)
	#receives human-readable lines with minimum length of 1 (by default is 4), and the searches	#for lines that start with = and have at least 1 to many = signs. The -E is for using the 	#extended regex version (if not defined we would be using BRE and we needed an escape '\' 	#symbol before +). Then we select the maximum length line which in this case is our answer. 	#We have used an AWK command (which is a scripting language related to bash). AWK is very 	#useful in string filtering and text searching. It is not just limited to bash and the 		#terminal. Learning AWK requires a tutorial itself but this command was obtained at a stack 	#over flow question after searching for the following question: "how to obtain the maximum 	#lengthed line from a file in the terminal".
	strings -n 1 data.txt | grep -E '^=+' | awk 'length > max_length { max_length = length; 	longest_line = $0 } END { print longest_line }'
	#the password in the file is: 
	G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s
level 11:
	ssh bandit10@bandit.labs.overthewire.org -p 2220
	#enter the password (G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s)
	# d stand for decoding.
	# read how base64 encoding and decoding is done manually, it is very interesting.
	# it can be found at the end of the following page:
	# https://www.base64encode.org/
	base64 -d data.txt | cat
	#the password in the file is:
	6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
level 12:
	ssh bandit11@bandit.labs.overthewire.org -p 2220
	#enter the password (6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM)
	#rotation 13 is an ancient ciphering algorithm.
	#it is simple and the deciphering and ciphering process is the same given that:
	#if you rotate a letter 13 times twice you will get the same letter (english alphabet has 26 letters).
	cat data.txt | tr '[a-z]' '[n-za-m]' | tr '[A-Z]' '[N-ZA-M]'
	#the password in the file is:
	JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
level 13:
	ssh bandit12@bandit.labs.overthewire.org -p 2220
	#enter the password (JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv)
	
