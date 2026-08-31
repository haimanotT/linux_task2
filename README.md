# Linux file permission and ownership 
written by: Haimanot Tadase
Assessment type: Linux fundamentals
Focus Area:
            -File creation
            -file permissions
            -ownership management
Environment:kalilinux
Date: aug 31 2026
###objective
To demonstrate practical understanding of Linux file permissions, ownership, and access control using standard Linux commands.

## step1 create a file
create a new file named secret.txt inside the linux_test directory by using the following command
###command:
cd linux_test used for move to linux_test directory
touch secret.txt to create new file inside linux test
ls to verify secret.txt was succeessfully created

<img width="260" height="228" alt="step1" src="https://github.com/user-attachments/assets/0cbe2b05-8499-488c-8e9b-529b4e39a450" />


##step2 Configure file permissions
### Command
chmod 640 secret.txt or chmod u=rw,g=r,o= secret.txt
ls -l secret.txt

The file permission was configured using the chmod command.
Permission value 640 is divided into three sections:

 Value  Permission  Applies To 
 6      Read + Write   Owner 
 4      Read Only      Group 
 0      No Permission  Others 


rw-r-----
allows the file owner to read and write file, allows group to read the file, and prevent access other users.
The ls -l command was used to verify that the permission settings were successfully applied.


<img width="233" height="126" alt="step2" src="https://github.com/user-attachments/assets/8d233a0e-e891-4757-a435-998c2b61914d" />

##step3  permission 640
Linux permissions are represented using three digits r-read =4,w-write-2 and x-excute=1 Each digit corresponds to a specific category of users
- Owner (User)
- Group
- Others
so 640 means
rw- read + write + no excute 4+2+0=6  the owner can read and write the  file but can't run or excute it
r-- read only 4+0+0=4  the group can read  the file but can't modify and excute it
--- no access 0+0+0=0 0thers users can't access the file

<img width="219" height="54" alt="Screenshot 2026-08-31 114417" src="https://github.com/user-attachments/assets/05662f9c-cab2-401b-a44f-e2c5b661d475" />

##step4 




            


