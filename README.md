# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/0661159e-07ed-4fc0-a623-f06eb2d2a11c)

cat < file2
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/703d2b2f-f9f7-46e3-8379-3c14e0f9f3d8)

# Comparing Files
cmp file1 file2
## OUTPUT

 ![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/2767eb0c-f66f-45ed-93e7-3a4c7b96f8d2)

comm file1 file2
 ## OUTPUT

 ![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/f717da3e-0f81-42a8-bfef-a6070c7e2a5f)

diff file1 file2
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/0284e169-b739-4c99-a5aa-aa6d86764ff5)

#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```


cut -c1-3 file11
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/d82fa44e-404f-441f-8174-22b913180dd8)

cut -d "|" -f 1 file22
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/84f293a4-597d-4365-a8ed-896626397832)

cut -d "|" -f 2 file22
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/f0f42839-97e1-4235-9b19-3174c7b44434)

cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/ff62afbc-ad70-44dc-afca-ed3d2cd59b3e)

grep hello newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/746e48f8-208b-4983-8475-fdc188d9de62)

grep -v hello newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/c5f9b352-a1bc-4017-b61c-aa3040b5634b)

cat newfile | grep -i "hello"
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/f0c24cac-cf75-468b-b7b0-71795e307de1)

cat newfile | grep -i -c "hello"
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/315983ef-6f08-494b-af66-b9c71b7f748e)

grep -R ubuntu /etc
## OUTPUT



grep -w -n world newfile   
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/0d79274f-d6a6-40ca-96ab-a791b207d9af)

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
egrep -w 'Hello|hello' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/7105877c-215a-46ba-9530-4805ba0f76a2)

egrep -w '(H|h)ello' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/e55a4047-8568-4acb-af1f-2f7ebe6714ef)

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/0056503c-9933-4289-b43b-6f502c1a5b3c)

egrep '(^hello)' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/56c514b4-2dd1-44d5-bf60-28e8a2278c95)

egrep '(world$)' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/458143f4-9356-4a70-ab8c-4aa711b8b9b0)

egrep '(World$)' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/7e0ea4c7-bbc8-498b-8224-1d545fa34be4)

egrep '((W|w)orld$)' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/6ef0f86f-cda3-4a1b-999d-485610bda42b)

egrep '[1-9]' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/eed9296a-b925-4d1c-9a5d-bd66df404b06)

egrep 'Linux.*world' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/84c3bf93-a5c4-425e-a030-b588642fec41)

egrep 'Linux.*World' newfile 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/ad9c5760-14ba-4af2-b3bb-ba2fb06e657f)

egrep l{2} newfile
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/43a2c95d-cdd7-4dd9-9c47-2742c1f2a1e4)


egrep 's{1,2}' newfile
## OUTPUT 

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/00d4967c-4193-4ca3-8d6c-ce526565e11d)


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```


sed -n -e '3p' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/fba54001-170f-42e8-9e6f-d97d3ce6bd45)

sed -n -e '$p' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/caab28b7-92a0-47f1-8d8a-d6b2b7e5721b)

sed  -e 's/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/2bfc6960-941e-419f-807d-58a7a4f9e336)


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/2e81d806-cb53-41e4-9eb9-9b3d66e0a5d3)


sed  '/tom/s/5000/6000/' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/620936d3-8bc3-4e28-9918-83605b04012e)


sed -n -e '1,5p' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/c04d3ab2-1cb7-41ed-8bd5-9ec16ce6b123)


sed -n -e '2,/Joe/p' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/e675a7ae-f2bf-4ffa-993a-69013ad55d6d)


sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/6139b82c-607f-4b24-a864-e0e1ec65bf5f)


seq 10 
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/ca305e1b-ade0-4525-97da-27c0b034b9dd)


seq 10 | sed -n '4,6p'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/31be3222-703c-4837-8c37-3dc9dc05cfcc)


seq 10 | sed -n '2,~4p'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/b76bd4e9-9a10-4212-aacc-5b70e71808dd)


seq 3 | sed '2a hello'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/ea9e99a6-1477-47fe-9445-2e46aeed6887)


seq 2 | sed '2i hello'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/85b9c987-76dc-4bf9-b67c-687a0e13bbd5)

seq 10 | sed '2,9c hello'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/9b719f61-6f02-4e2f-996c-b3a4751d1549)


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/3179a220-580d-4375-ac42-6db74c24cdf5)


sed -n '2,4{s/$/*/;p}' file23
# OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/c22518e3-23c7-4985-98bd-73d2db416ac6)

#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/dcdbe459-fce7-4fd0-9220-225562d1c75b)


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/64184661-ee68-47f1-8023-2bd3b15e7308)


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/0ef1cd08-905d-4508-b6d6-6805a87d3bbd)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/fede2576-2fba-4663-a30c-bbc6a3e41fa4)

 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/1d256c7c-645c-44ae-94c0-b43742db5136)


#Backup commands
tar -cvf backup.tar *
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/be3022b8-cd04-456c-915b-f3244f11a9e8)


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT

![image](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/5fe44737-6f37-4e70-b9ef-353d7f59dc77)


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 ```
argshift1.sh   file11        fornested1.sh  OS-Linux-commands-Shell-script
argshift.sh    file2         funcex.sh      palindrome.sh
backupdir      file21        herecheck.txt  psswdperm.sh
backup.tar.gz  file22        ifcompound.sh  scriptest.sh
casecheck.sh   file23        ifnested1.sh   strcomp.sh
cities         forbreak.sh   ifnested.sh    untiltest.sh
data.dat       forctype.sh   iftest.sh      urllist.txt
elifcheck.sh   forin1.sh     my-script.sh   whiletest
exread1.sh     forin2.sh     nc.awk         whiletest.sh
exread.sh      forin3.sh     newfile
file1          forinfile.sh  one 
gunzip backup.tar.gz
```
## OUTPUT
```
argshift1.sh   file11        fornested1.sh  OS-Linux-commands-Shell-script
argshift.sh    file2         funcex.sh      palindrome.sh
backupdir      file21        herecheck.txt  psswdperm.sh
backup.tar.gz  file22        ifcompound.sh  scriptest.sh
casecheck.sh   file23        ifnested1.sh   strcomp.sh
cities         forbreak.sh   ifnested.sh    untiltest.sh
data.dat       forctype.sh   iftest.sh      urllist.txt
elifcheck.sh   forin1.sh     my-script.sh   whiletest
exread1.sh     forin2.sh     nc.awk         whiletest.sh
exread.sh      forin3.sh     newfile
file1          forinfile.sh  one
(base) sec@sec-ThinkPad-E15-Gen-4:~/os/ex01/backupdir$ gunzip backup.tar.gz
(base) sec@sec-ThinkPad-E15-Gen-4:~/os/ex01/backupdir$ ls
argshift1.sh  file11        fornested1.sh  OS-Linux-commands-Shell-script
argshift.sh   file2         funcex.sh      palindrome.sh
backupdir     file21        herecheck.txt  psswdperm.sh
backup.tar    file22        ifcompound.sh  scriptest.sh
casecheck.sh  file23        ifnested1.sh   strcomp.sh
cities        forbreak.sh   ifnested.sh    untiltest.sh
data.dat      forctype.sh   iftest.sh      urllist.txt
elifcheck.sh  forin1.sh     my-script.sh   whiletest
exread1.sh    forin2.sh     nc.awk         whiletest.sh
exread.sh     forin3.sh     newfile
file1         forinfile.sh  one
```
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

![1](https://github.com/mithra916/OS-Linux-commands-Shell-script/assets/149986612/001789dd-0327-4df4-b836-147cfbfe943c)


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
```
./scriptest.sh: line 1: #!/bin/sh: No such file or directory
“File name is ./scriptest.sh ”
File name is  scriptest.sh
“First arg. is ” 1
“Second arg. is ” 2
“Third arg. is ” 3
“Fourth arg. is ”
The $@ is  1 2 3
The $\# is  1#
The $$ is  14337
    PID TTY          TIME CMD
  13614 pts/1    00:00:00 bash
  14337 pts/1    00:00:00 bash
  14340 pts/1    00:00:00 ps
```
ls file1
## OUTPUT
```
file1
echo $?
```
## OUTPUT 
```
0
./one
bash: ./one: Permission denied
echo $?
```
## OUTPUT 
```
127
abcd
 ```
echo $?
 ## OUTPUT
 ```
127
```
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT
chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
```
./strcomp.sh: line 1: #!/bin/bash: No such file or directory
baseball is less than hockey
./strcomp.sh: line 10: ^d: command not found
```
# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
bash: ./psswdperm.sh: Permission denied
# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT
```
./ifnested.sh: line 1: #!/bin/bash: No such file or directory
“/home/sec The object exists, is it a file?”
“No,/home/sec it is not a file!”
“But /home/sec/.bash_history is a file!”
./ifnested.sh: line 18: ^d: command not found
```
# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
```
./elifcheck.sh: line 1: #!/bin/bash: No such file or directory
Sorry, you are not allowed here
```
# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
```
./ifcompound.sh: line 1: #!/bin/bash: No such file or directory
The file exists and you can write to it
```

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
```
./ifcompound.sh: line 1: #!/bin/bash: No such file or directory
The file exists and you can write to it
```
# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
```
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT
```
Starting loop 1:
Inside loop: 1
Inside loop: 2
Inside loop: 3
Starting loop 2:
Inside loop: 1
Inside loop: 2
Inside loop: 3
Starting loop 3:
Inside loop: 1
Inside loop: 2
Inside loop: 3
```
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT
```
Enter your name: Venkatanathan
Hello Venkatanathan, welcome to my program.
```
$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT
```
Enter your name: Venkatanathan
Hello Venkatanathan, welcome to my program.
```

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT
```
Enter your name: Venkatanathan
./exread1.sh: line 4: unexpected EOF while looking for matching `"'
./exread1.sh: line 5: syntax error: unexpected end of file
```

$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 
```
bash: ./funcex.sh: Permission denied
```
 
 ./funcex.sh 1 2
```
bash: ./funcex.sh: Permission denied
```
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 ```
+ ((  3  ))
+ echo 1
1
+ shift
+ ((  2  ))
+ echo 2
2
+ shift
+ ((  1  ))
+ echo 3
3
+ shift
+ ((  0  ))
+ set +x
```
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 ```
1
2
3
```
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 ```
+ ((  3  ))
+ echo 1
1
+ shift
+ ((  2  ))
+ echo 2
2
+ shift
+ ((  1  ))
+ echo 3
3
+ shift
+ ((  0  ))
+ set +x
```
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 ```
 7 	 bcdfghj
8 	 abcdfghj
7 	 bcdfghj
8 	 ebcdfghj
7 	 bcdfghj
8 	 ibcdfghj
7 	 bcdfghj
8 	 obcdfghj
7 	 bcdfghj
8 	 ubcdfghj
total characters 75
Number of Lines are 10
No of Words count: 10
```
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 
```
Enter the number
45
Number is NOT palindrome
```

# RESULT:
The Commands are executed successfully.
