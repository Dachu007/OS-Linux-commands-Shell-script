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

<img width="351" height="102" alt="Screenshot from 2026-01-30 20-35-29" src="https://github.com/user-attachments/assets/d1b6910f-526d-4263-878b-013df2e369eb" />


cat < file2
## OUTPUT
<img width="355" height="118" alt="Screenshot from 2026-01-30 20-35-48" src="https://github.com/user-attachments/assets/172426b8-05d8-4222-be52-4e83ea858f9e" />


# Comparing Files
cmp file1 file2
## OUTPUT
 <img width="353" height="47" alt="Screenshot from 2026-01-30 20-36-01" src="https://github.com/user-attachments/assets/b2e49f7f-ae9e-4a09-82b2-25890628f7d4" />

comm file1 file2
 ## OUTPUT
<img width="376" height="144" alt="Screenshot from 2026-01-30 20-36-46" src="https://github.com/user-attachments/assets/e40d4fb1-6141-4c06-a142-6817ca6aa6a2" />

 
diff file1 file2
## OUTPUT
<img width="378" height="188" alt="Screenshot from 2026-01-30 20-37-16" src="https://github.com/user-attachments/assets/8a32c44e-46aa-4972-95bd-886a00742ba1" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
<img width="378" height="79" alt="Screenshot from 2026-01-30 20-39-12" src="https://github.com/user-attachments/assets/6f316998-31ef-469b-b3fe-752161ea27c9" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
<img width="380" height="165" alt="Screenshot from 2026-01-30 20-39-23" src="https://github.com/user-attachments/assets/2f130863-da4c-4f4a-8c21-04f4cdacee44" />


cut -c1-3 file11
## OUTPUT

<img width="368" height="67" alt="Screenshot from 2026-01-30 20-39-36" src="https://github.com/user-attachments/assets/dccc4592-5562-4e63-9767-332ed6add203" />



cut -d "|" -f 1 file22
## OUTPUT

<img width="444" height="72" alt="Screenshot from 2026-02-02 09-36-54" src="https://github.com/user-attachments/assets/026ac906-85b5-4757-b135-22f5fd66c03a" />


cut -d "|" -f 2 file22
## OUTPUT
<img width="440" height="80" alt="Screenshot from 2026-01-30 20-40-23" src="https://github.com/user-attachments/assets/b90ca1fd-780e-4fa2-8af7-f30978410665" />


cat < newfile 
```
Hello world
hello world
^d
````
<img width="438" height="68" alt="Screenshot from 2026-01-30 20-42-43" src="https://github.com/user-attachments/assets/1906e300-3894-4dbf-9e05-ba8706687bd8" />

cat > newfile 
Hello world
hello world

 <img width="425" height="67" alt="Screenshot from 2026-01-30 20-44-40" src="https://github.com/user-attachments/assets/b068b21d-a7ee-4550-be91-7a8378ef19bc" />

grep Hello newfile 
## OUTPUT
<img width="486" height="77" alt="Screenshot from 2026-01-30 20-45-30" src="https://github.com/user-attachments/assets/a826eee2-1e8c-4859-b3c5-381be0c287ca" />



grep hello newfile 
## OUTPUT


<img width="486" height="77" alt="Screenshot from 2026-01-30 20-45-30" src="https://github.com/user-attachments/assets/c7938b21-f2c9-4bb4-97f0-b6a2f788c9db" />


grep -v hello newfile 
## OUTPUT
<img width="494" height="45" alt="Screenshot from 2026-01-30 20-46-10" src="https://github.com/user-attachments/assets/108ce8f8-742f-4cae-8261-769a00c702fa" />



cat newfile | grep -i "hello"
## OUTPUT

<img width="570" height="67" alt="Screenshot from 2026-01-30 20-47-12" src="https://github.com/user-attachments/assets/72f56adf-0769-4b56-b932-a5505e923352" />



cat newfile | grep -i -c "hello"
## OUTPUT

<img width="603" height="51" alt="Screenshot from 2026-01-30 20-48-06" src="https://github.com/user-attachments/assets/b6f649a2-fe64-4b46-8dda-3fcd5d862259" />



grep -R ubuntu /etc
## OUTPUT
<img width="1457" height="1108" alt="Screenshot from 2026-01-30 20-49-36" src="https://github.com/user-attachments/assets/72f2cd94-e17d-49e4-8e8c-bf6a78b0213c" />



grep -w -n world newfile   
## OUTPUT

<img width="720" height="66" alt="Screenshot from 2026-01-30 20-50-19" src="https://github.com/user-attachments/assets/7de84f2d-6a9a-4fe5-8274-184eace5151e" />

cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
<img width="712" height="123" alt="Screenshot from 2026-01-30 20-52-58" src="https://github.com/user-attachments/assets/84e52769-be37-4e2b-b15e-74f113314690" />

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
<img width="717" height="144" alt="Screenshot from 2026-01-30 20-53-40" src="https://github.com/user-attachments/assets/84413d52-919b-4d04-976a-656fdd30958c" />

egrep -w 'Hello|hello' newfile 
## OUTPUT
<img width="706" height="68" alt="Screenshot from 2026-01-30 20-55-07" src="https://github.com/user-attachments/assets/e1cc06c3-78b3-49c5-a36a-7c3d01587b47" />



egrep -w '(H|h)ello' newfile 
## OUTPUT

<img width="706" height="67" alt="Screenshot from 2026-01-30 20-55-51" src="https://github.com/user-attachments/assets/14ecdbdf-6ee7-404b-9d93-bde711a6ca12" />


egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
<img width="709" height="66" alt="Screenshot from 2026-01-30 20-56-36" src="https://github.com/user-attachments/assets/b58262fd-6ff1-4a17-84e5-932af12e72e2" />




egrep '(^hello)' newfile 
## OUTPUT
<img width="709" height="66" alt="Screenshot from 2026-01-30 20-57-16" src="https://github.com/user-attachments/assets/ca4add5e-1000-4108-89b8-a4f8870aa41e" />



egrep '(world$)' newfile 
## OUTPUT
<img width="709" height="66" alt="Screenshot from 2026-01-30 20-57-57" src="https://github.com/user-attachments/assets/9532c4a1-64dc-497f-9ea7-ca801d616b01" />



egrep '(World$)' newfile 
## OUTPUT
<img width="692" height="49" alt="Screenshot from 2026-01-30 20-58-36" src="https://github.com/user-attachments/assets/7017bd88-eaae-4917-bb4e-432d9f505418" />


egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="700" height="98" alt="Screenshot from 2026-01-30 20-59-30" src="https://github.com/user-attachments/assets/b7afd632-7a41-47dd-8382-000990d53600" />


egrep '[1-9]' newfile 
## OUTPUT
<img width="692" height="45" alt="Screenshot from 2026-01-30 21-00-12" src="https://github.com/user-attachments/assets/58ce72ba-c615-4b37-9d1f-5b7e612c8a96" />



egrep 'Linux.*world' newfile 
## OUTPUT
<img width="686" height="49" alt="Screenshot from 2026-01-30 21-00-44" src="https://github.com/user-attachments/assets/95bd635d-41e1-41b2-9d1d-bd8c20f9c7ed" />


egrep 'Linux.*World' newfile 
## OUTPUT
<img width="689" height="46" alt="Screenshot from 2026-01-30 21-01-43" src="https://github.com/user-attachments/assets/89d8a4aa-6f55-406a-aa40-5f9585be5447" />


egrep l{2} newfile
## OUTPUT
<img width="684" height="66" alt="Screenshot from 2026-01-30 21-02-54" src="https://github.com/user-attachments/assets/1dcc7b77-c743-4a83-8094-d577e9157952" />



egrep 's{1,2}' newfile
## OUTPUT 
<img width="685" height="87" alt="Screenshot from 2026-01-30 21-02-19" src="https://github.com/user-attachments/assets/5dab14e7-93de-4504-aa4d-835a1e52eefe" />


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
<img width="672" height="173" alt="Screenshot from 2026-01-30 21-03-59" src="https://github.com/user-attachments/assets/3b7c5315-f8a6-419e-88a9-c3ee06489263" />


sed -n -e '3p' file23
## OUTPUT

<img width="652" height="53" alt="Screenshot from 2026-01-30 21-04-43" src="https://github.com/user-attachments/assets/9460d8c6-52db-49c0-80f0-6dd693ab0206" />


sed -n -e '$p' file23
## OUTPUT

<img width="650" height="46" alt="Screenshot from 2026-01-30 21-05-09" src="https://github.com/user-attachments/assets/3c941ca7-7b96-486c-828f-94d01a61e49e" />


sed  -e 's/Ram/Sita/' file23
## OUTPUT

<img width="650" height="174" alt="Screenshot from 2026-01-30 21-06-24" src="https://github.com/user-attachments/assets/18c68ebb-8449-4b14-88e9-24dcf874a246" />


sed  -e '2s/Ram/Sita/' file23
## OUTPUT
<img width="650" height="171" alt="Screenshot from 2026-01-30 21-09-06" src="https://github.com/user-attachments/assets/8ead1067-8126-4205-817f-26b30b1c555b" />



sed  '/tom/s/5000/6000/' file23
## OUTPUT
<img width="654" height="174" alt="Screenshot from 2026-01-30 21-07-25" src="https://github.com/user-attachments/assets/f176e6c7-f140-48be-8384-70256964fe02" />



sed -n -e '1,5p' file23
## OUTPUT

<img width="643" height="122" alt="Screenshot from 2026-01-30 21-08-31" src="https://github.com/user-attachments/assets/cd0829d2-a740-4d22-9c27-e6589171296e" />


sed -n -e '2,/Joe/p' file23
## OUTPUT

<img width="649" height="79" alt="Screenshot from 2026-01-30 21-10-44" src="https://github.com/user-attachments/assets/0c2e8a8e-8b5c-4eec-a7e0-ba9cf35d202e" />



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
<img width="640" height="61" alt="Screenshot from 2026-01-30 21-10-13" src="https://github.com/user-attachments/assets/e0738a51-6efd-40b2-8bc5-69bc9d81c963" />



seq 10 
## OUTPUT

<img width="641" height="204" alt="Screenshot from 2026-01-30 21-11-01" src="https://github.com/user-attachments/assets/8d5d5ed5-caa2-4688-b6cd-06f7f3860458" />


seq 10 | sed -n '4,6p'
## OUTPUT

<img width="618" height="82" alt="Screenshot from 2026-01-30 21-11-30" src="https://github.com/user-attachments/assets/5239b323-d0dc-4b44-91fd-b08faa4ad2a4" />


seq 10 | sed -n '2,~4p'
## OUTPUT

<img width="619" height="79" alt="Screenshot from 2026-01-30 21-11-54" src="https://github.com/user-attachments/assets/85b8960d-c8d3-4912-8749-2ceb1a759961" />


seq 3 | sed '2a hello'
## OUTPUT
<img width="611" height="114" alt="Screenshot from 2026-01-30 21-12-19" src="https://github.com/user-attachments/assets/2df3383b-52b5-46c3-b1f9-fd2fcb69831e" />



seq 2 | sed '2i hello'
## OUTPUT
<img width="609" height="80" alt="Screenshot from 2026-01-30 21-12-56" src="https://github.com/user-attachments/assets/9cbaef79-e070-4b14-af83-790566540f73" />


seq 10 | sed '2,9c hello'
## OUTPUT
<img width="609" height="80" alt="Screenshot from 2026-01-30 21-13-14" src="https://github.com/user-attachments/assets/19f9a176-5000-441c-985f-1ee92b3f56bf" />


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

<img width="610" height="75" alt="Screenshot from 2026-01-30 21-13-29" src="https://github.com/user-attachments/assets/808ed24e-c32b-4c42-ac1e-858ac8f7e418" />


sed -n '2,4{s/$/*/;p}' file23
<img width="614" height="76" alt="Screenshot from 2026-01-30 21-13-50" src="https://github.com/user-attachments/assets/9dcaed8a-d1e0-4f1b-aafd-83b2ceeb81f1" />


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

<img width="618" height="122" alt="Screenshot from 2026-01-30 21-14-30" src="https://github.com/user-attachments/assets/fcd3595a-a5d9-4ca1-8301-17e531dcf15d" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
```
<img width="606" height="129" alt="Screenshot from 2026-01-30 21-15-02" src="https://github.com/user-attachments/assets/2e816740-3893-4531-9506-4240fc1161c7" />

uniq file22
## OUTPUT

<img width="604" height="119" alt="Screenshot from 2026-01-30 21-15-22" src="https://github.com/user-attachments/assets/cbc5b9c4-d7f0-42ed-8c69-2208017a2925" />


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
<img width="653" height="174" alt="Screenshot from 2026-01-30 21-15-39" src="https://github.com/user-attachments/assets/34d5f8b8-8e51-4421-9b49-636d57d30eb3" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
<img width="638" height="84" alt="Screenshot from 2026-01-30 21-17-34" src="https://github.com/user-attachments/assets/dcd8283d-95e7-48e1-90e9-1f5ad2c7671d" />

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
<img width="615" height="78" alt="Screenshot from 2026-01-30 21-18-15" src="https://github.com/user-attachments/assets/799ffbd5-90ab-46e1-b043-dc719a8a0782" />

cat urllist.txt | tr -d ' '
 ## OUTPUT
<img width="608" height="85" alt="Screenshot from 2026-01-30 21-18-44" src="https://github.com/user-attachments/assets/b0f7d761-4128-4ae3-9236-1d4dc6c07c7f" />


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
<img width="678" height="87" alt="Screenshot from 2026-01-30 21-19-23" src="https://github.com/user-attachments/assets/71f721e4-f1c1-4d70-9311-71f42f984e93" />



#Backup commands
tar -cvf backup.tar *
## OUTPUT
<img width="659" height="551" alt="Screenshot from 2026-01-30 21-19-48" src="https://github.com/user-attachments/assets/57df6909-9247-406a-907a-30a857fd25c0" />


mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 <img width="625" height="48" alt="Screenshot from 2026-01-30 21-20-18" src="https://github.com/user-attachments/assets/39441464-1580-42c7-80b4-ecd0a7ef27fe" />

tar -tvf backup.tar
## OUTPUT
<img width="558" height="144" alt="Screenshot from 2026-02-02 09-16-13" src="https://github.com/user-attachments/assets/fdf8ea24-235d-4921-9c61-87fdbab4c559" />


tar -xvf backup.tar
## OUTPUT
<img width="541" height="30" alt="Screenshot from 2026-02-02 09-21-34" src="https://github.com/user-attachments/assets/7c856bdf-b421-415f-84a1-76e79f368027" />

gzip backup.tar

ls .gz
## OUTPUT
 <img width="450" height="28" alt="Screenshot from 2026-02-02 09-22-11" src="https://github.com/user-attachments/assets/f93e8aeb-0432-4279-9024-85d05afb6364" />
 <img width="463" height="22" alt="Screenshot from 2026-02-02 09-22-20" src="https://github.com/user-attachments/assets/8f0c0163-4d7b-4274-90f1-3ca3f2ee0aec" />


gunzip backup.tar.gz
## OUTPUT
<img width="561" height="30" alt="Screenshot from 2026-02-02 09-21-24" src="https://github.com/user-attachments/assets/413b23c7-3307-42b5-ad78-7def89b3c51d" />

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
<img width="310" height="69" alt="315052332-b482cca7-8962-4860-b090-01c2f7d5631f" src="https://github.com/user-attachments/assets/019b098b-1410-4fc0-8350-9743e9659857" />

<img width="724" height="57" alt="315052369-1b3717e7-816c-4559-9162-ba1bcc381389" src="https://github.com/user-attachments/assets/5f67d4f6-a9c0-4fc6-88bc-3b21fe4f9e39" />

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```


cat herecheck.txt
## OUTPUT
<img width="829" height="93" alt="315052480-8d87f8c1-ec1f-40bf-ae3d-a238cdae7f1e" src="https://github.com/user-attachments/assets/389eac45-fab1-4f48-b678-a405f915c1f5" />

<img width="829" height="93" alt="315052480-8d87f8c1-ec1f-40bf-ae3d-a238cdae7f1e" src="https://github.com/user-attachments/assets/f2e41583-a972-4145-a231-d4607fb39818" />


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

 <img width="747" height="220" alt="315052611-c588b9fa-70fb-46e2-b813-890537ed1ed3" src="https://github.com/user-attachments/assets/d67e15bb-64af-4dec-8b92-8fcc1c1f367e" />
 
<img width="747" height="220" alt="315052650-2e16bd60-d505-4007-b33f-56db9624a4e9" src="https://github.com/user-attachments/assets/0e4fd75a-6c08-4233-9ccc-8a61d807580f" />

<img width="786" height="294" alt="315052758-5231a559-d457-4144-9049-3cc26942878f" src="https://github.com/user-attachments/assets/d2c42e9b-552a-49d7-bcc6-04b309c22537" />

ls file1
## OUTPUT
<img width="267" height="42" alt="315052815-1afa9eff-1dd2-4cb6-9c04-0f1a5c4dbaad" src="https://github.com/user-attachments/assets/94beccb0-0830-4d6a-97ff-0d140200edf0" />

echo $?
## OUTPUT 
<img width="267" height="42" alt="315052865-2e61fc4c-c3cc-4d53-8ac2-8699b8848d6b" src="https://github.com/user-attachments/assets/5ebf86dc-3c41-4a02-8fc2-236c641a34c8" />
./one bash: ./one: Permission denied



 
echo $?
## OUTPUT 
 <img width="267" height="42" alt="315052865-2e61fc4c-c3cc-4d53-8ac2-8699b8848d6b" src="https://github.com/user-attachments/assets/320c2e9b-8170-4c92-ab60-d3add295ebe6" />

abcd
 
echo $?
 ## OUTPUT
<img width="267" height="42" alt="315052968-b2683246-7732-419a-9aa6-9b83bd1a3f62" src="https://github.com/user-attachments/assets/6a6bf78f-8689-489b-acd9-6139c975a6b6" />


 
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
## OUTPUT
<img width="328" height="183" alt="315053021-f9c4c7d3-3f51-4654-96c8-1089fd444799" src="https://github.com/user-attachments/assets/43db2df1-a2b7-4b58-b18a-c78720484476" />



chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

<img width="376" height="62" alt="315053044-c3e6a3d1-5768-47df-bb8e-b4d5e1ee6f6a" src="https://github.com/user-attachments/assets/68f0fe36-2b21-4444-bfa2-278121691359" />

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
<img width="544" height="255" alt="315053084-4bc0833c-4767-48eb-b442-f8de40d1ba95" src="https://github.com/user-attachments/assets/faa1f25d-e2f8-4387-9553-81d45607d321" />

<img width="511" height="42" alt="315053112-a9f06f33-d615-494c-aeeb-772da14700cd" src="https://github.com/user-attachments/assets/c515efdf-1417-49fa-9a36-014a642e1949" />

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
<img width="421" height="617" alt="315053156-387b2b9f-6946-482f-9a13-5cdefbcbdd1a" src="https://github.com/user-attachments/assets/a56327e5-e7fb-433a-af6f-4c8175e9d3fa" />

<img width="410" height="77" alt="315053182-055e38c0-5d0e-442e-9a36-59c4797fd3e1" src="https://github.com/user-attachments/assets/0480c60c-9aeb-4720-859a-aa2f98b08b09" />


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
## OUTPUT
 <img width="421" height="471" alt="315053263-483b0887-bd1e-4eb6-9591-08ecec1fc41e" src="https://github.com/user-attachments/assets/1a8d1eee-119a-436b-9ae5-8fee195e02d3" />
 
<img width="421" height="81" alt="315053314-03f55e4e-a4a2-4e90-9c0b-87b39075f66e" src="https://github.com/user-attachments/assets/6552d2eb-42a9-4ec5-8277-b707d98398ac" />

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
## OUTPUT
<img width="421" height="615" alt="315053446-325ec43b-4197-462d-94c4-9d9657961af2" src="https://github.com/user-attachments/assets/52139e58-a449-4a01-ab5d-ef6f89437551" />

<img width="421" height="130" alt="315053469-83a0241b-4020-430b-9a7a-202965b054f5" src="https://github.com/user-attachments/assets/4f6bf77a-673c-4580-9a98-b5ac4eeee06f" />

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
<img width="504" height="327" alt="315053514-bcc634bc-5954-4232-90aa-05be0d3d1ca0" src="https://github.com/user-attachments/assets/be021e77-b443-4e0d-8707-9432a29a786f" />

<img width="420" height="60" alt="315053538-c4c90885-c2f1-4718-ae16-65a530a98edc" src="https://github.com/user-attachments/assets/6b49625a-46ae-4945-88cc-877ad57ad7d2" />


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
<img width="430" height="182" alt="315053566-a41b9a13-0f5e-42d0-a411-0fb590cd5671" src="https://github.com/user-attachments/assets/a5f4bbd7-e9bd-4523-9e68-a7e21cb080c4" />

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
 <img width="528" height="272" alt="315183094-71cc9ac9-051e-4f13-bfb3-ec66612cee3f" src="https://github.com/user-attachments/assets/0a484669-ae6f-4422-b05b-99717b93daaa" />

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
 <img width="576" height="401" alt="315183482-15ebf32c-fbd1-4e33-8530-7b77bd53c75d" src="https://github.com/user-attachments/assets/36d3ce63-8d3e-44a8-8ca8-882299464c13" />

 
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
<img width="397" height="241" alt="315184570-9130f11b-7819-4a41-8fd4-57cff80b6ca9" src="https://github.com/user-attachments/assets/5d04da1b-25a2-4096-8918-b90c20e5ca2f" />

$ chmod 755 untiltest.sh
 
 
 <img width="367" height="148" alt="315185489-87df45c8-b2a7-4cbd-897b-e024ec0c1de0" src="https://github.com/user-attachments/assets/fe743025-8384-4a96-bd83-a42947c91476" />

cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 <img width="573" height="92" alt="315184855-0a3743d0-8c59-4c10-bf0e-2cd411f5a494" src="https://github.com/user-attachments/assets/0e40bf57-661a-4691-88e6-a09a431c8272" />

$ chmod 755 forin1.sh
 <img width="372" height="183" alt="315185864-60624a1d-3322-40f2-a790-f3ee3a89485f" src="https://github.com/user-attachments/assets/56c4c646-5882-464d-aca0-0d2f35eba017" />

 
cat forin2.sh 
<img width="372" height="183" alt="315186482-5db7c59d-3bfc-4284-822d-d06f00ff1435" src="https://github.com/user-attachments/assets/203f3419-5bc0-476a-8939-8e73356de8b5" />

```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 <img width="399" height="237" alt="315186981-7701db5e-5306-425a-9d5d-012edd323a05" src="https://github.com/user-attachments/assets/33b4365d-1dd7-4c89-8622-883726f51d72" />

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

 <img width="399" height="237" alt="315186981-7701db5e-5306-425a-9d5d-012edd323a05" src="https://github.com/user-attachments/assets/dd54fc7e-2c26-42ee-976d-c2c35bbd46aa" />

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
<img width="345" height="148" alt="315187046-587f8b75-9e7b-42fb-abe6-ee595a8aa805" src="https://github.com/user-attachments/assets/93a2103b-577e-419b-ab08-aad2aaad8983" />

<img width="399" height="271" alt="315187081-8b1fd7ea-f2b6-43ca-9197-6f6036c19ac2-1" src="https://github.com/user-attachments/assets/5118a2f1-d0e5-41e0-8a88-d5454ecbf374" />


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

 <img width="402" height="423" alt="315187265-24658c9b-c66b-4fe2-9eb2-a556f73de444" src="https://github.com/user-attachments/assets/5c864128-db7d-40a1-a945-99afd54205b5" />

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
<img width="402" height="275" alt="315187365-24fe1758-0ec0-41b7-8fa5-ca31c39c85b1" src="https://github.com/user-attachments/assets/85ae170a-4d6e-4467-94af-74d3434c814c" />

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

<img width="421" height="311" alt="315187407-6a9303d1-a881-47ed-bd9d-099ef3c21dbc" src="https://github.com/user-attachments/assets/70040e1e-6d33-46ab-be1a-b1f4e436a3ab" />

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

<img width="421" height="190" alt="315187449-85ce33d2-6012-4571-ab07-2cfa54eb95f0" src="https://github.com/user-attachments/assets/607e640e-823a-477b-8dd0-ba59e9d97df7" />


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
<img width="421" height="328" alt="315187596-ebd3ec88-ada0-4d86-b1e5-abe28f1a6b7a" src="https://github.com/user-attachments/assets/7f138a33-81ed-4d5a-b1e1-f8613e8d2946" />

 
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

 <img width="421" height="206" alt="315187633-ccb7ee05-e9c1-4592-92ec-6f67e8b7f853" src="https://github.com/user-attachments/assets/fe593b42-eb26-48ae-8ee8-2ab4c6007f82" />

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

 <img width="400" height="202" alt="315187689-c736a718-56b3-4417-a87c-f86a1c6a818f" src="https://github.com/user-attachments/assets/7a54a70e-e3a4-4cee-ae50-b9318baf162d" />

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
 <img width="381" height="239" alt="315187795-d7850997-0a34-4786-a55a-9f89853f7664" src="https://github.com/user-attachments/assets/29c6b31a-43ca-4a5b-8401-c7e080cbfdb5" />

 
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

<img width="381" height="205" alt="315187843-af6b4b57-0562-4499-bdeb-970163211290" src="https://github.com/user-attachments/assets/05c26272-97a4-4a48-b2de-29b63b7e6b87" />

awk -f nc.awk data.dat

## OUTPUT 

 <img width="425" height="744" alt="315187905-2774c0cd-c926-4206-8350-29d39440505c" src="https://github.com/user-attachments/assets/0b0fc9b2-8345-4fb4-b24a-ad8a8b188e60" />

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
<img width="400" height="492" alt="315187941-37b5c6c2-d570-451c-bd4a-9fb00b0c8ef2" src="https://github.com/user-attachments/assets/e9c8f6fc-6aef-4273-bae0-e241be4f8bc6" />


# RESULT:
The Commands are executed successfully.
