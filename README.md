# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting
# NAME : UDHAYAMOORTHY A
# REG NO: 212225040477

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

<img width="422" height="181" alt="627043824-85c3764f-65ca-43a5-824a-6914300a9b51" src="https://github.com/user-attachments/assets/1c815c8c-ab50-4c5a-875c-2a31a9e596bc" />

cat < file2
## OUTPUT

<img width="382" height="197" alt="627044005-5d9e0ce6-8661-42fe-a86a-b98427fa8270" src="https://github.com/user-attachments/assets/daf5844e-66af-4d34-b40c-9cc0765e5116" />

# Comparing Files
cmp file1 file2
## OUTPUT

 <img width="426" height="95" alt="627044245-00828879-46e6-4622-b056-ea1a970b2ba1" src="https://github.com/user-attachments/assets/0e94ffb8-5d62-46d2-903b-6bb53de80fdc" />

comm file1 file2
 ## OUTPUT

 <img width="550" height="292" alt="627044504-ad47e135-1c08-4ba6-8c20-cd0195fa95a6" src="https://github.com/user-attachments/assets/a3e6d828-fe72-4c96-bede-4225a4f5a16e" />

diff file1 file2
## OUTPUT

<img width="455" height="317" alt="627044721-19c310b8-8818-4afe-b60f-ce390e0a3665" src="https://github.com/user-attachments/assets/30a7842e-2a26-4994-a47d-918ee3d50cb7" />

#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
# output

<img width="415" height="92" alt="627045737-1bc131dc-7120-46d8-99d6-ef56f0cd0f79" src="https://github.com/user-attachments/assets/ea3f288c-7192-4c14-8b11-da26143e7d19" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
# output

<img width="437" height="127" alt="627045905-b731a65e-5614-4e09-a001-05b541242a06" src="https://github.com/user-attachments/assets/092c312f-784c-4d14-92a5-a61adf00626f" />

cut -c1-3 file11
## OUTPUT

<img width="421" height="107" alt="627046047-dee9e8ec-43b6-4744-9ac1-51f263ea34ce" src="https://github.com/user-attachments/assets/15a76925-873d-48c0-94ee-d19df418d281" />

cut -d "|" -f 1 file22
## OUTPUT


<img width="425" height="127" alt="627046323-d815891d-1fbf-4d4d-b701-624f7c1364ce" src="https://github.com/user-attachments/assets/80899347-fc2a-49fd-8e4d-2928fdd7b1ba" />

cut -d "|" -f 2 file22
## OUTPUT

<img width="366" height="122" alt="627046605-b9048550-afb9-428d-b986-626f20325e9a" src="https://github.com/user-attachments/assets/fea8386a-c6cb-4029-a601-dcd106b6d403" />

cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 
Hello world
hello world
 # output 

 <img width="437" height="112" alt="627047418-158d920b-6b0c-4485-9b47-72a3c5d97a80" src="https://github.com/user-attachments/assets/5b5e7394-51cc-4f79-b38d-efeb6fb4311f" />

grep Hello newfile 
## OUTPUT

<img width="327" height="76" alt="627050385-b5bc6b48-9ef8-4123-9b2f-c2a2bda45df0" src="https://github.com/user-attachments/assets/8c7d745d-8220-42d7-aa50-04c2902d9357" />

grep hello newfile 
## OUTPUT

<img width="277" height="137" alt="627051371-51638577-c272-461f-97f8-34dc7476e844" src="https://github.com/user-attachments/assets/4e421d37-fe39-4698-a0c1-a93b87a0ec51" />

grep -v hello newfile 
## OUTPUT

<img width="362" height="77" alt="627051621-63c5b410-455a-4a02-9b02-1c6f4e4bcec6" src="https://github.com/user-attachments/assets/83b0fc58-7815-4a8a-bdec-35d2906fb424" />

cat newfile | grep -i "hello"
## OUTPUT

<img width="502" height="171" alt="627052060-60636515-374b-4009-8fa2-ad7990264bfd" src="https://github.com/user-attachments/assets/4913eab1-88ca-4c7e-85be-6307ab93d3c7" />

cat newfile | grep -i -c "hello"
## OUTPUT

<img width="476" height="81" alt="627052392-be97679d-1a7f-473a-8939-093ede1decbf" src="https://github.com/user-attachments/assets/31d328ca-dab0-409b-aa89-39de63233bf6" />

grep -R ubuntu /etc
## OUTPUT

<img width="801" height="557" alt="627052806-ae09ecc8-ebfa-4669-9361-f397f6e0b84f" src="https://github.com/user-attachments/assets/4615c55c-bea6-4077-9a2a-94cc25dd27ef" />

grep -w -n world newfile   
## OUTPUT

<img width="422" height="132" alt="627053344-e27121b6-44a4-471f-be12-42ff8c8d08cb" src="https://github.com/user-attachments/assets/10fa018a-2f5c-468f-8010-1e3e7dab8a76" />

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
 ## OUTPUT

 <img width="502" height="347" alt="627053973-69a62b1e-f677-4a9b-b98a-4115bc444250" src="https://github.com/user-attachments/assets/56229de1-db28-4b1e-8413-3e8dc1edcf19" />

egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="451" height="131" alt="627054203-3d1dcac4-54e0-4663-aacb-fcbe92c2c439" src="https://github.com/user-attachments/assets/bae155aa-1257-400c-806b-23c04d1d8615" />

egrep -w '(H|h)ello' newfile 
## OUTPUT

<img width="616" height="152" alt="627258404-aeaa6a14-8deb-4095-a395-1ad2528d5455" src="https://github.com/user-attachments/assets/7ee717cb-d1e7-4c1e-9cd3-2b89a86c46f6" />

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

<img width="462" height="107" alt="627273649-ce8b77e5-076a-4bdc-bd26-503d1d705449" src="https://github.com/user-attachments/assets/be6c1d28-cbdd-4b1c-b1f8-9c192b18c927" />

egrep '(^hello)' newfile 
## OUTPUT

<img width="446" height="81" alt="627273893-d4df2506-9ba6-4a7f-9be3-b02114a2c4fe" src="https://github.com/user-attachments/assets/da67fcc5-465b-47a4-a5dc-21157fadac6f" />

egrep '(world$)' newfile 
## OUTPUT

<img width="452" height="110" alt="627274168-3a4c5b2f-521b-48ee-92f0-1023e643f121" src="https://github.com/user-attachments/assets/ca7b02e5-0db3-41bd-a8bb-dc8a16e7cbc6" />

egrep '(World$)' newfile 
## OUTPUT

<img width="481" height="80" alt="627274362-97119d37-0589-4811-9205-139fb2a125a2" src="https://github.com/user-attachments/assets/66a18ac6-072b-4a3e-8544-523ee71e3645" />

egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="502" height="137" alt="627274604-9c1b0ea0-a206-4a2e-867e-e70da3c41580" src="https://github.com/user-attachments/assets/f61b3c21-ef69-4f60-8303-4b06c8c4232f" />

egrep '[1-9]' newfile 
## OUTPUT

<img width="511" height="82" alt="627274757-3b821cd8-f37c-4f23-84cd-b35cf2e6cbfb" src="https://github.com/user-attachments/assets/881d54f9-e3d7-4310-aba6-85ef3f7adc3f" />

egrep 'Linux.*world' newfile 
## OUTPUT


egrep 'Linux.*World' newfile 
## OUTPUT



egrep l{2} newfile
## OUTPUT



egrep 's{1,2}' newfile
## OUTPUT 


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



sed -n -e '$p' file23
## OUTPUT



sed  -e 's/Ram/Sita/' file23
## OUTPUT



sed  -e '2s/Ram/Sita/' file23
## OUTPUT



sed  '/tom/s/5000/6000/' file23
## OUTPUT



sed -n -e '1,5p' file23
## OUTPUT



sed -n -e '2,/Joe/p' file23
## OUTPUT




sed -n -e '/tom/,/Joe/p' file23
## OUTPUT



seq 10 
## OUTPUT



seq 10 | sed -n '4,6p'
## OUTPUT



seq 10 | sed -n '2,~4p'
## OUTPUT



seq 3 | sed '2a hello'
## OUTPUT



seq 2 | sed '2i hello'
## OUTPUT


seq 10 | sed '2,9c hello'
## OUTPUT


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT



sed -n '2,4{s/$/*/;p}' file23


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



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

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


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT



#Backup commands
tar -cvf backup.tar *
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 
gunzip backup.tar.gz
## OUTPUT

 
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

 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT


 
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


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



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

 
 ./funcex.sh 1 2

 
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

 <img width="472" height="381" alt="630006750-41aee01c-ddae-4604-8dc6-ea7e392d3c16" src="https://github.com/user-attachments/assets/3abd223c-c0b7-4c0d-886c-f05586f83d9e" />

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

<img width="590" height="185" alt="630007348-ac9c13f5-8ad4-4f9d-9e84-ff7c2a6288a3" src="https://github.com/user-attachments/assets/13ca678a-8631-418c-b471-3f8002860f02" />

# RESULT:
The Commands are executed successfully.
