# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

# Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

# Step 2:

Execute the following commands

# Step 3:

Testing the commands for the desired output. 

# COMMANDS:
# Create the following files file1, file2 as follows:
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
# Display the content of the files

cat < file1
### OUTPUT

<img width="302" height="161" alt="image" src="https://github.com/user-attachments/assets/d0bf1d38-1f27-4b99-9c97-7d5811698b3a" />

cat < file2
### OUTPUT

<img width="292" height="178" alt="image" src="https://github.com/user-attachments/assets/586a12bb-4210-4250-ab57-9428959ab42c" />


# Comparing Files

cmp file1 file2
### OUTPUT

 <img width="377" height="82" alt="image" src="https://github.com/user-attachments/assets/7fa1419f-d029-462a-906a-d0ccb1e0b54d" />


comm file1 file2
### OUTPUT

<img width="471" height="304" alt="Screenshot 2025-09-23 144626" src="https://github.com/user-attachments/assets/6d24d213-dc1d-4ad1-ab1d-4172fc70286e" />

diff file1 file2
### OUTPUT

<img width="357" height="302" alt="image" src="https://github.com/user-attachments/assets/5fc13f07-18ff-4bac-8735-3ff282d0c98f" />


# Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```

<img width="323" height="117" alt="image" src="https://github.com/user-attachments/assets/8f434094-5437-4c2b-92bc-f7fecb1b1ddc" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```

<img width="363" height="150" alt="image" src="https://github.com/user-attachments/assets/5d528c58-6fe4-4c35-a1f0-7b4c1acbe591" />

cut -c1-3 file11
### OUTPUT

<img width="273" height="107" alt="image" src="https://github.com/user-attachments/assets/318d5940-7876-409e-b626-3d1e8240d26e" />


cut -d "|" -f 1 file22
### OUTPUT

<img width="345" height="132" alt="image" src="https://github.com/user-attachments/assets/d5be3981-74ee-4356-baf6-78bf205170b1" />

cut -d "|" -f 2 file22
### OUTPUT

<img width="407" height="147" alt="image" src="https://github.com/user-attachments/assets/f30b2e15-1a00-4a07-a8fe-95f7fb549a17" />




cat < newfile 
```
Hello world
hello world
^d
````
cat > newfile 

<img width="315" height="113" alt="image" src="https://github.com/user-attachments/assets/33dab457-77c8-4980-bc30-fe5450baf895" />


grep Hello newfile 
### OUTPUT

<img width="305" height="154" alt="image" src="https://github.com/user-attachments/assets/051857ab-c991-408c-a2ee-42e820682866" />

grep hello newfile 
### OUTPUT

<img width="297" height="85" alt="image" src="https://github.com/user-attachments/assets/9cf37d03-eed2-406b-adae-95b976750a32" />

grep -v hello newfile 
### OUTPUT

<img width="321" height="88" alt="image" src="https://github.com/user-attachments/assets/920e0225-d379-4800-9229-925d82e1db6b" />

cat newfile | grep -i "hello"
### OUTPUT

<img width="412" height="113" alt="image" src="https://github.com/user-attachments/assets/d0f7b742-7134-45b6-a23a-7bf90d6acd8b" />


cat newfile | grep -i -c "hello"
### OUTPUT

<img width="423" height="77" alt="image" src="https://github.com/user-attachments/assets/6cdf5d7d-18ae-47eb-a69d-757cd012f543" />

grep -R ubuntu /etc
### OUTPUT

<img width="786" height="153" alt="image" src="https://github.com/user-attachments/assets/00ad44df-3796-4f2b-917b-638718b1d7cf" />
<img width="937" height="803" alt="image" src="https://github.com/user-attachments/assets/6085a580-448a-4965-9d81-2b3fff02ae31" />
<img width="944" height="849" alt="image" src="https://github.com/user-attachments/assets/5574a8f6-4542-4a08-a4b2-663b7fed80ce" />
<img width="946" height="821" alt="image" src="https://github.com/user-attachments/assets/bf3d7b20-2aa5-48e0-8f6f-d5f40a4ffe91" />
<img width="938" height="852" alt="image" src="https://github.com/user-attachments/assets/f480f374-f79c-4484-9612-c37adaaf5ada" />
<img width="935" height="854" alt="image" src="https://github.com/user-attachments/assets/f1051f44-b171-4adf-9be7-b03f484607e3" />



grep -w -n world newfile   
### OUTPUT

<img width="335" height="98" alt="image" src="https://github.com/user-attachments/assets/f1cd68e7-705d-4040-bff4-9dd67f9f0042" />


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

<img width="347" height="173" alt="image" src="https://github.com/user-attachments/assets/c6fa42df-aa59-4765-9490-87efdf289fac" />


egrep -w 'Hello|hello' newfile 
### OUTPUT

<img width="422" height="107" alt="image" src="https://github.com/user-attachments/assets/822b9e78-99c4-4ff3-914d-969a95c43c1d" />


egrep -w '(H|h)ello' newfile 
### OUTPUT

<img width="405" height="102" alt="image" src="https://github.com/user-attachments/assets/472f3ba4-6a21-4b31-9d9c-3b2e0ed3ef40" />


egrep -w '(H|h)ell[a-z]' newfile 
### OUTPUT

<img width="430" height="102" alt="image" src="https://github.com/user-attachments/assets/ae43e391-1a00-4fb1-97cd-598d4ee792b6" />


egrep '(^hello)' newfile 
### OUTPUT

<img width="387" height="75" alt="image" src="https://github.com/user-attachments/assets/bb0b1b25-9eca-4f5b-a6ed-8c187a51e0a7" />


egrep '(world$)' newfile 
### OUTPUT

<img width="367" height="98" alt="image" src="https://github.com/user-attachments/assets/91b95a9f-a012-4170-8523-c174e94b19bf" />


egrep '(World$)' newfile 
### OUTPUT

<img width="347" height="82" alt="image" src="https://github.com/user-attachments/assets/2bed95e2-0f3c-49b4-a0d8-0a45f49f53b6" />


egrep '((W|w)orld$)' newfile 
### OUTPUT

<img width="397" height="123" alt="image" src="https://github.com/user-attachments/assets/9e09e517-cb49-4c75-b10a-c351f3e7777c" />


egrep '[1-9]' newfile 
### OUTPUT

<img width="365" height="76" alt="image" src="https://github.com/user-attachments/assets/8f4a078a-58d9-4f8c-9e74-454582b1bb54" />


egrep 'Linux.*world' newfile 
### OUTPUT

<img width="370" height="75" alt="image" src="https://github.com/user-attachments/assets/72c77094-f577-456b-b2ea-ea1de64786a0" />


egrep 'Linux.*World' newfile 
### OUTPUT

<img width="362" height="75" alt="image" src="https://github.com/user-attachments/assets/8849fb3b-a739-4a47-95e1-c28f8b96486e" />


egrep l{2} newfile
### OUTPUT

<img width="340" height="108" alt="image" src="https://github.com/user-attachments/assets/b4aa6eb7-7ca2-4d1a-971e-299be4b0834e" />


egrep 's{1,2}' newfile
### OUTPUT 

<img width="340" height="127" alt="image" src="https://github.com/user-attachments/assets/ca5e6daa-2090-4fd8-95a8-4d3a6f7ea20e" />


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
### OUTPUT

<img width="391" height="276" alt="Screenshot 2025-09-23 150759" src="https://github.com/user-attachments/assets/d03d004c-7f92-4fd2-9dce-66480b5bb577" />

sed -n -e '3p' file23
### OUTPUT

<img width="323" height="82" alt="image" src="https://github.com/user-attachments/assets/32cec2d1-e8da-4dc7-8bb9-dc3f146c6dd1" />


sed -n -e '$p' file23
### OUTPUT

<img width="314" height="61" alt="Screenshot 2025-09-23 181217" src="https://github.com/user-attachments/assets/f3f486df-01a8-427e-bf58-82150a3c4b6d" /> 

<img width="306" height="30" alt="Screenshot 2025-09-23 181239" src="https://github.com/user-attachments/assets/69afda3b-69db-4bc7-945f-b62b436425f0" />



sed -e '2s/Ram/Sita/' file23

### OUTPUT

<img width="387" height="266" alt="Screenshot 2025-09-23 150945" src="https://github.com/user-attachments/assets/32b33f61-5a4f-443e-b205-ef05317b0130" />


sed  -e '2s/Ram/Sita/' file23
### OUTPUT

<img width="387" height="266" alt="Screenshot 2025-09-23 150945" src="https://github.com/user-attachments/assets/a7591cd7-9a9c-496a-852d-77fa8773ac99" />


sed  '/tom/s/5000/6000/' file23
### OUTPUT

<img width="411" height="267" alt="Screenshot 2025-09-23 151135" src="https://github.com/user-attachments/assets/c2391917-0063-4d00-b883-3ffb89d2af72" />


sed -n -e '1,5p' file23
### OUTPUT

<img width="385" height="185" alt="image" src="https://github.com/user-attachments/assets/8135a9fc-3780-46c4-bc03-d44c84bc6dac" />


sed -n -e '2,/Joe/p' file23
### OUTPUT

<img width="366" height="130" alt="image" src="https://github.com/user-attachments/assets/5954a958-211a-40a6-95e9-157b964ec5aa" />


sed -n -e '/tom/,/Joe/p' file23
### OUTPUT

<img width="406" height="127" alt="image" src="https://github.com/user-attachments/assets/5921e180-28a7-47fa-976b-e2bc7088f6d2" />


seq 10 | sed -n '4,6p'
### OUTPUT

<img width="408" height="120" alt="image" src="https://github.com/user-attachments/assets/cb51027e-5c87-4053-bb19-c272e781c954" />


seq 10 | sed -n '2,~4p'
### OUTPUT

<img width="370" height="108" alt="image" src="https://github.com/user-attachments/assets/9b6bdbde-53bb-4755-a5ee-89549c0a58fa" />


seq 3 | sed '2a hello'
### OUTPUT

<img width="342" height="147" alt="image" src="https://github.com/user-attachments/assets/89b4c799-3cc9-4075-90dd-57ea7a692458" />


seq 2 | sed '2i hello'

### OUTPUT

<img width="327" height="126" alt="image" src="https://github.com/user-attachments/assets/1ee20d2e-a56b-4bc2-9d27-3c9de09904fc" />


seq 10 | sed '2,9c hello'
### OUTPUT

<img width="377" height="127" alt="image" src="https://github.com/user-attachments/assets/d3425fa4-b8f0-4d89-a6f9-49d21b6f72b8" />


sed -n '2,4{s/^/$/;p}' file23
### OUTPUT

<img width="392" height="131" alt="image" src="https://github.com/user-attachments/assets/d2091bca-5777-4735-9faa-5499156487f7" />


sed -n '2,4{s/$/*/;p}' file23
### OUTPUT

<img width="415" height="127" alt="image" src="https://github.com/user-attachments/assets/4fc3ebcf-6cb0-4411-81ae-373b38642d2c" />


#Sorting File content

cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
### OUTPUT

<img width="372" height="181" alt="image" src="https://github.com/user-attachments/assets/f58ffd89-7c3d-41df-aa73-00de291b52a6" />


sort file21
### OUTPUT

<img width="363" height="200" alt="image" src="https://github.com/user-attachments/assets/74c23156-726d-4f4e-9652-5266814a9983" />


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
### OUTPUT

<img width="357" height="215" alt="image" src="https://github.com/user-attachments/assets/9628c9f7-df69-484e-be2b-f0651a068dcd" />


uniq file22
### OUTPUT

<img width="337" height="186" alt="image" src="https://github.com/user-attachments/assets/7e482f55-ac65-46bb-956e-2814cbcf3c0c" />


#Using tr command

cat file23 | tr [:lower:] [:upper:]
### OUTPUT

<img width="438" height="260" alt="image" src="https://github.com/user-attachments/assets/b8f3d45b-97e2-4046-9f1b-3faeb01787dc" />


cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat < urllist.txt

<img width="340" height="147" alt="Screenshot 2025-09-23 153404" src="https://github.com/user-attachments/assets/ad0473b2-3350-4c71-a1d9-b10ee8d35efc" />


cat > urllist.txt
'''
www. yahoo. com
www. google. com
www. mrcet.... com
'''

cat urllist.txt | tr -d ' '

### OUTPUT

<img width="334" height="135" alt="Screenshot 2025-09-23 153605" src="https://github.com/user-attachments/assets/8f23a622-c29d-49ff-b7db-744ac723de27" />

 
cat urllist.txt | tr -d ' ' | tr -s '.'

### OUTPUT

<img width="509" height="136" alt="Screenshot 2025-09-23 153825" src="https://github.com/user-attachments/assets/609c4653-467c-4bc1-a97d-5c89c847fa40" />


#Backup commands

tar -cvf backup.tar *
### OUTPUT

<img width="365" height="461" alt="Screenshot 2025-09-23 153853" src="https://github.com/user-attachments/assets/bcf833bc-c304-4243-8eff-ac15adfe9a53" />


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
### OUTPUT

<img width="577" height="308" alt="image" src="https://github.com/user-attachments/assets/4e17e16d-5d9b-4eb3-aab7-d8b29e9a7440" />


tar -xvf backup.tar
### OUTPUT


<img width="408" height="467" alt="Screenshot 2025-09-23 154120" src="https://github.com/user-attachments/assets/2215e519-f027-4d5e-bf54-68f1f8841924" />

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
### OUTPUT

 <img width="395" height="361" alt="Screenshot 2025-09-23 154802" src="https://github.com/user-attachments/assets/0ca8a2eb-7fde-4116-a697-c8ae17c188e4" />

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
### OUTPUTcd 

<img width="374" height="149" alt="Screenshot 2025-09-23 154744" src="https://github.com/user-attachments/assets/57d2478f-f0a4-4e47-8c3b-b86c9e333c0c" />



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

<img width="395" height="361" alt="Screenshot 2025-09-23 154802" src="https://github.com/user-attachments/assets/8e466a5c-833e-4219-9602-982ea9cb39ba" />

chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

### OUTPUT

<img width="686" height="450" alt="Screenshot 2025-09-23 154955" src="https://github.com/user-attachments/assets/f417c950-c2fb-401c-b78b-c0459f2b2a02" />

ls file1
### OUTPUT

<img width="320" height="86" alt="image" src="https://github.com/user-attachments/assets/4b70da08-ca2b-481c-9793-317fb9bc5eb9" />


echo $?
### OUTPUT 

<img width="342" height="77" alt="image" src="https://github.com/user-attachments/assets/7dcf9fa8-9e29-4ea8-8c76-5322fa7ed83f" />


# mis-using string comparisons

cat > strcomp.sh 
```bash
#!/bin/bash
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
#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
### OUTPUT


<img width="426" height="281" alt="Screenshot 2025-09-23 155410" src="https://github.com/user-attachments/assets/b1430e91-dbb6-463a-ae9c-e4cb5e57b28b" />

chmod 755 strcomp.sh
 
./strcomp.sh 
### OUTPUT

<img width="395" height="137" alt="Screenshot 2025-09-23 155436" src="https://github.com/user-attachments/assets/0492fa22-d5b9-45ba-a895-e7d5bc32582a" />


# check file ownership
cat > psswdperm.sh 
```bash
#!/bin/bash
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
#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
### OUTPUT

<img width="621" height="353" alt="Screenshot 2025-09-23 155837" src="https://github.com/user-attachments/assets/1f8479ff-06a5-4d16-81ea-2d78768570d0" />


# check if with file location
cat>ifnested.sh 
```bash
#!/bin/bash
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
#!/bin/bash
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
### OUTPUT

<img width="545" height="478" alt="Screenshot 2025-09-23 155921" src="https://github.com/user-attachments/assets/5a8d4ca1-3832-4b28-a4ca-21bd1e49cb92" />


# using numeric test comparisons
cat > iftest.sh 
```bash
#!/bin/bash
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
#!/bin/bash
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

<img width="541" height="382" alt="Screenshot 2025-09-23 160157" src="https://github.com/user-attachments/assets/6523ae86-c2e1-437a-9bff-0891b74c9d0c" />


$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT

<img width="463" height="155" alt="Screenshot 2025-09-23 160211" src="https://github.com/user-attachments/assets/2d7e9421-1727-4735-ad04-a743ef14defe" />


# check if a file
cat > ifnested.sh 
```bash
#!/bin/bash
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
#!/bin/bash
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

<img width="537" height="176" alt="Screenshot 2025-09-23 160013" src="https://github.com/user-attachments/assets/f6788330-1b79-4e4e-8509-afe775695e11" />


# looking for a possible value using elif
cat > elifcheck.sh 
```bash
#!/bin/bash
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

<img width="550" height="431" alt="Screenshot 2025-09-23 160410" src="https://github.com/user-attachments/assets/bf706b4c-81b9-4e0e-a1e1-3a2b7ced0343" />


$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
### OUTPUT

<img width="353" height="107" alt="Screenshot 2025-09-23 160522" src="https://github.com/user-attachments/assets/10288d60-fe63-4d4b-9a32-ec81fbebd21a" />


# testing compound comparisons
cat> ifcompound.sh 
```bash
#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
### OUTPUT

<img width="560" height="353" alt="image" src="https://github.com/user-attachments/assets/2a8e6147-0162-4c05-a6fb-3e6c3e2d27bb" />


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
### OUTPUT

<img width="559" height="381" alt="Screenshot 2025-09-23 160943" src="https://github.com/user-attachments/assets/783a9c50-9981-4edd-99bc-a15369ee32d5" />


cat > whiletest
```bacd
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```

<img width="353" height="217" alt="Screenshot 2025-09-23 161501" src="https://github.com/user-attachments/assets/6acb8e48-9fcc-4f6d-8efb-14448ac00f3b" />


$ chmod 755 whiletest.sh
$ ./whiletest.sh

### OUTPUT

<img width="329" height="300" alt="Screenshot 2025-09-23 161510" src="https://github.com/user-attachments/assets/f0c0350d-39b6-408f-b55c-18ad22359551" />


cat > untiltest.sh 
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
 
$ ./untiltest.sh

### OUTPUT

<img width="492" height="378" alt="Screenshot 2025-09-23 162540" src="https://github.com/user-attachments/assets/f7b8ea34-2d95-4b04-b859-2f4f944a2174" />


cat > forin1.sh 
```bash
#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
$ ./forin1.sh

### OUTPUT

<img width="629" height="402" alt="Screenshot 2025-09-23 162646" src="https://github.com/user-attachments/assets/fc3ff22b-91d2-4741-a08e-11f305fc943d" />


cat > forin2.sh 
```bash
#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat > forin2.sh 
```bash
#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 

# OUPUT

<img width="515" height="335" alt="Screenshot 2025-09-23 162735" src="https://github.com/user-attachments/assets/413b129d-75eb-4653-88df-74feb38cb986" />


cat > forin3.sh 
```bash
#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 

### OUTPUT

<img width="511" height="400" alt="Screenshot 2025-09-23 162819" src="https://github.com/user-attachments/assets/8677a87a-81ab-469f-ac1c-3e503c65c1e0" />

cat > forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh
$ ./forin1.sh

### OUTPUT

<img width="629" height="402" alt="Screenshot 2025-09-23 162646" src="https://github.com/user-attachments/assets/a4ed79b3-b7be-48ef-87f8-680c820696d7" />


cat > forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file"
done
```
$ chmod 777 forinfile.sh
$ cat > cities
```
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam
```
### OUTPUT

<img width="361" height="275" alt="Screenshot 2025-09-23 163014" src="https://github.com/user-attachments/assets/f2243664-0376-4e14-b451-600b7455276a" />


cat > forctype.sh 
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

### OUTPUT

<img width="342" height="356" alt="Screenshot 2025-09-23 163211" src="https://github.com/user-attachments/assets/e2a00ab7-74ae-43c1-a232-3526d946f3ef" />


cat > forctype1.sh 
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

### OUTPUT

<img width="419" height="362" alt="Screenshot 2025-09-23 163442" src="https://github.com/user-attachments/assets/f6874226-2dbb-4492-8f1e-0b2fe7f9671c" />


cat > fornested1.sh 
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

### OUTPUT

<img width="287" height="391" alt="Screenshot 2025-09-23 163746" src="https://github.com/user-attachments/assets/0a84e8a5-ef7e-4e08-8afd-c14ba1eb1b46" />


cat > forbreak.sh 
```bash
#!/bin/bash
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed"
```

$ chmod 755 forbreak.sh
$ ./forbreak.sh 

### OUTPUT

<img width="261" height="270" alt="Screenshot 2025-09-23 170131" src="https://github.com/user-attachments/assets/fff53e5d-8872-4572-a8af-65c4f6a4ee06" />

 
cat > forcontinue.sh 
```bash
#!/bin/bash

for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed"
```

 
$ chmod 755 forcontinue.sh

$ ./forcontinue.sh 

### OUTPUT

<img width="274" height="310" alt="Screenshot 2025-09-23 170504" src="https://github.com/user-attachments/assets/c7867a5f-704f-40a8-9ab6-b47d3420a9e9" />


cat > exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 

### OUTPUT

<img width="293" height="187" alt="Screenshot 2025-09-23 170610" src="https://github.com/user-attachments/assets/6c1f9e7a-49cf-4679-8032-c40f416220bf" />


 cat > exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. "
``` 
$ chmod 755 exread1.sh 
$ ./exread1.sh 
### OUTPUT

<img width="296" height="171" alt="Screenshot 2025-09-23 170707" src="https://github.com/user-attachments/assets/5bf7af1f-4854-487a-acfa-823ec55de0d7" />

 
cat > funcex.sh
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

$ chmod 755 funcex.sh
$ ./funcex.sh 
$ ./funcex.sh 1 2
### OUTPUT


cat > argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh
$ ./argshift.sh 1 2 3

### OUTPUT

 

 cat > argshift1.sh
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
$ ./argshift.sh 1 2 3

### OUTPUT



cat > argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```

$ chmod 777 argshift.sh
$ ./argshift.sh 1 2 3
### OUTPUT
 
 

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
### OUTPUT 



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
$ chmod 777 palindrome.sh
$ ./palindrome.sh

### OUTPUT 




# RESULT:
The Commands are executed successfully.
