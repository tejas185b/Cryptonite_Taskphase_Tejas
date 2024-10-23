# Cryptonite_Taskphase_Tejas
## Hello Hackers
### Intro to Commands
- write hello to execute that command
- Command: hello
- Flag: pwn.college{E0521KYlc8R23FFIbDQwzey3chg.ddjNyUDLxIjN0czW}
### Intro to Arguments
- use argument hackers with the hello command
- Command: hello hackers
- Flag: pwn.college{kYaLDnokj_iNvJtSNlyUr8XHQ7N.dhjNyUDLxIjN0czW} 
## Pondering Paths
### THE ROOT
- Process: to open a directory write its path
- Command: /pwn
- Flag:  pwn.college{8HPX0ULgOquFhvtOD_iOTUk8Hkn.dhzN5QDLxIjN0czW}
### PROGRAM AND ABSOLUTE PATHS
- Process: to open a directory write its path
- Command: /challenge/run
- Flag:  pwn.college{QLM7_ap1MOeH-JU4s7s_ml_8Uos.dVDN1QDLxIjN0czW}
### POSITION THY SELF
- Process: use cd(change directory) which changes the current directory
- Command: cd /var , /challenge/run
- Flag:  pwn.college{4u3GJM-buI8oV_ti8NRz9XffSu}s.dZDN1QDLxIjN0czW
### POSITION ELSEWHERE
- Process: use cd(change directory) which changes the current directory
- Command: cd / , /challenge/run
- Flag:  pwn.college{EWoeXlVQ4vdyP46QVDwqiqVEBJ4.ddDN1QDLxIjN0czW}
### POSITION YET ELSEWHERE
- Process: enter /challenge/run it will give you error and the actuat path then use that path to access flag
- Command: cd /usr/bin , /challenge/run
- Flag:  pwn.college{YBd0nhBOTAdjDd-1ukd5FafIzzD.dhDN1QDLxIjN0czW}
### IMPLICIT RELATIVE PATHS, FROM /
- Process: go to / directory and execute /challenge/run
- Command: cd / , challenge/run
- Flag:   pwn.college{YbdH-yLsCFtYHloHqBeCHsIkxdG.dlDN1QDLxIjN0czW}
### EXPLICIT RELATIVE PATHS, FROM /
- Process: Go to / directory and from there use that directory itself to go to /challenge/run
- Command: cd / , ./challenge/run
- Flag:   pwn.college{ILGu7MMAnLtJ1csfg4BOFa94rDd.dBTN1QDLxIjN0czW}
### IMPLICIT RELATIVE PATH
- Process: Use . to execute /challenge/run from the current directory
- Command: cd /challenge , ./run
- Flag:   pwn.college{sjx5kpR2EelN3rzLYKeDuZyXzNx.dFTN1QDLxIjN0czW}
### HOME SWEET HOME
- Process: Use ~ this to access the path of current directory and pass an argument like "~/x" to /challenge/run
- Command: /challenge/run ~/x
- Flag:   pwn.college{c82TyGxCtBkWkPkXX_69kykIKWa.dNzM4QDLxIjN0czW}
## COMPREHENDING COMMANDS
### cat: not the pet, but the command!
- Process: use the command 'cat' with filename argument to read its contents and display
- Command: cat flag
- Flag: pwn.college{8pzXN1hImdZMh35GssvsCQ-PbbP.dFzN1QDLxIjN0czW}
### catting absolute paths
- Process: use the command 'cat' and argument as absolute path "/flag"
- Command: cat /flag
- Flag: pwn.college{EPgyh3lcdhVzV8u0xbT8AIJrsRI.dlTM5QDLxIjN0czW}
### More catting practice
- Process: Find the path of flag and pass the full path as argument to cat
- Command:  cat /lib/x86_64-linux-gnu/perl-base/flag
- Flag:  pwn.college{o8iUvXXSTewotpatROcTeNtjP0o.dBjM5QDLxIjN0czW}
### Grepping for a needle in the haystack
- Process: search for string "pwn" using grep command in /challenge/data.txt file
- Command: grep pwn.college /challenge/data.txt
- Flag: pwn.college{IOnFhH4xFzFgxnomCkecG0hTGuI.ddTM4QDLxIjN0czW}
### Listing files
- Process: list the items in /challenge using ls and then execute the changed name of run file to get the flag
- Command: ls /challenge  ,  /challenge/21454-renamed-run-13820
- Flag: pwn.college{AsINvXH0Xi-uyorPNqhCr1aq8PH.dhjM4QDLxIjN0czW}
### Touching files
- Process: Create two files using touch command and then execute /challenge/run
- Command: touch /tmp/pwn , touch /tmp/college , /challenge/run
- Flag: pwn.college{Yy3mhFSZo5MUy_QUWU-2IeyeKRH.dBzM4QDLxIjN0czW}
### Removing files
- Process: Remove the "delete_me" file using rm command
- Command: rm delete_me
- Flag: pwn.college{IQoHMithP_sIPgTdZC4cq6tmRvi.dZTOwUDLxIjN0czW}
### Hidden files
- Process: find the hidden file in / using -a after the command ls and then read the file using cat
- Command: ls / -a
- Flag: pwn.college{0ntK67L1VeMjp1UK494-eITFOKa.dBTN4QDLxIjN0czW}
### An epic filesystem quest
- Process: Use the commmand cd,ls,ls -a,cat and follow the hints and clues to access the flag
- Command: cat /usr/local/lib/python3.8/dist-packages/sympy/functions/elementary/tests/.NOTE
- Flag: pwn.college{wSicPpF9Ic6ywPZOwoqL5ieuQeA.dljM4QDLxIjN0czW}
### Making directories
- Process: Make a directory using mkdir and then create file inside it using touch named college
- Command: mkdir /tmp/pwn , touch /tmp/pwn/college
- Flag: pwn.college{czVjkA8qPofgsBPhV_NICtr4qJG.dFzM4QDLxIjN0czW}
### Finding files
- Process: use find / -name flag to find all flag directories and files and then use hit and trial to find the actual flag which was found in /opt/linux/linux-5.4/drivers/usb/gadget/function/flag
- Command: find / -name flag
- Flag: pwn.college{I-biMHXa2Q2Sg0p-XwJw9Y8753w.dJzM4QDLxIjN0czW} 
### Linking files
- Process: link /flag to /not-the-flag so that it executes /flag when it tries to execute /not-the-flag
- Command: ln -s /flag /home/hacker/not-the-flag
- Flag: pwn.college{QrERiCzjsML5-rA5VeG_HIjeZSb.dlTM1UDLxIjN0czW}

## DIGESTING DOCUMENTATION
### Learning from Documentation
- Process: pass --giveflag as argument to /challenge/challenge
- Command: /challenge/challenge –giveflag
- Flag: pwn.college{Iwy-Gz_nK0CMUUbaIdZo5f1jr8u.dRjM5QDLxIjN0czW}
### Learning complex Usage
- Process: Pass the argumet /flag to argument --printfile as /flag is the place where all the hidden files are present
- Command: /challenge/challenge --printfile /flag
- Flag: pwn.college{cIJLz7eLeWZAMtgMDAXZDmV-f6A.dVjM5QDLxIjN0czW}
### Reading Manuals
- Process: read the entire manual below the exact argument is given to pass to /challenge/challenge to get flag
- Command: /challenge/challenge --wunetp 862
- Flag: pwn.college{wuP8P6Gnetp-ma2RGe41v2KZN6p.dRTM4QDLxIjN0czW}
### Searching Manuals
- Process: Search in the manual for flag word it will give you the argument
- Command: /challenge/challenge --vsdo
- Flag: pwn.college{kOklujL48_J6H0izRTL_L0akP4M.dVTM4QDLxIjN0czW}
### Searching for manuals
- Process: use the commend man -k challenge to find the keyword challenge in all man files and then find flag argument
- Command:  man man , man -k challenge, /challenge/challenge  --qwzxtv 587
- Flag: pwn.college{MPq-XGMw5zKx87tEBv0GaCVVBnj.dZTM4QDLxIjN0czW}
### Helpful programs
- Process: first execute /challege/challenge --help it gives its all arguments then we pass -p argument to it get our secret number and then pass the argument --give-the-flag 486 to /challenge/challenge
- Command: /challenge/challenge -p , /challenge/challenge --give-the-flag 856
- Flag: pwn.college{Eg8Oc5nX6-DyBZvWItJzhNUvI65.ddjM4QDLxIjN0czW}
### Help for bulletins
- Process: First pass challenge to help we see all its shells and over there 'secret' value is given use that to access flag
- Command: help challenge , challenge --secret "c4J6eioo"
- Flag: pwn.college{c4J6eiooBebte4zY3f6NEVAJfSB.dRTM5QDLxIjN0czW}
## FILE GLOBBING  

### Matching with *
- Process: pass the argument /c* to cd which change the directory to /challenge and then execute /challenge/run using ./r*
- Command: cd /c* ,  ./r*
- Flag: pwn.college{4zlJlzCX2e1UuTh2T8dKHXa6sH6.dFjM4QDLxIjN0czW}
### Matching with ?
- Process: pass the argument /?ha??enge to cd and then execute /challenge/run
- Command: cd /?ha??enge  , /challenge/run
- Flag: pwn.college{w2jNRscLs3MaKJ2vD4msaEVEV5m.dJjM4QDLxIjN0czW}
### Matching with []
- Process: change directory to /challenge/files and then execute /challenge/run file_[bash]
- Command: cd /challenge/files , /challenge/run file_[bash]
- Flag: pwn.college{Uf9e3GifLkQUgl1p1Mbi1eOY7DZ.dNjM4QDLxIjN0czW}
### Matching paths with []
- Process: execute /challenge/run followed by absolute path of files
- Command: /challenge/run /challenge/files/file_[bash]
- Flag: pwn.college{8umgoH0iUC_iXSsk01hNdH0cLCc.dRjM4QDLxIjN0czW}
### Mixing globs
- Process: execute the line [cep]*
- Command: cd /challenge/files , /challenge/run [cep]*
- Flag: pwn.college{4SLqVmWA9nY8V-5ZLKHgqLRONKO.dVjM4QDLxIjN0czW}
### Exclusionary globbing
- Process: Execute the line /challenge/run [!pwn]*
- Command: cd /challenge/files , 	/challenge/run [!pwn]*
- Flag: pwn.college{USAJHRT2a9ZPxIuj3rsuRBArm20.dZjM4QDLxIjN0czW}
## PRACTICING PIPING
### Redirecting piping
- Process: echo output PWN to file COLLEGE
- Command: echo PWN > COLLEGE
- Flag: pwn.college{cQY5cM_6j50SN2X6vW4bm6hmSBi.dRjN1QDLxIjN0czW}
### Redirecting more output
- Process: push output to variable and cat it
- Command: /challenge/run > myflag , cat myflag
- Flag: pwn.college{ERKcCgHvdR9solH9s9JDBa-Zsai.dVjN1QDLxIjN0czW}
### Appending output
- Process: append /challenge/run to my-flag using >>
- Command: /challenge/run >> ~/the-flag , cat the-flag
- Flag: pwn.college{QQ6r9CZAg3KeWFrr2mWgZAKaz2J.ddDM5QDLxIjN0czW}
### Redirecting errors
- Process: Redirect Errors to instructions and output to myflag and then cat myflag
- Command: /challenge/run > myflag 2> instructions
- Flag: pwn.college{UvMEyqMnzmX32X7DIIBbnkNoMdt.ddjN1QDLxIjN0czW}
### Redirecting input
- Process: First echo the word College to PWN and then redirect it to /challenge/run
- Command: echo COLLEGE > PWN , /challenge/run < PWN
- Flag: pwn.college{8ye5GfV26XTqeuUE3iXNET3sihk.dBzN1QDLxIjN0czW}
### Grepping stored stored
- Process: First direct the output of /challenge/run to tmp/data.txt and then grep the word pwn
- Command: /challenge/run > /tmp/data.txt , grep pwn.college /tmp/data.txt
- Flag: pwn.college{4sJq9ehenpNHpRAqLmVk16NgF-A.dhTM4QDLxIjN0czW}
### Grepping live output
- Process: execute /challenge/run and grep pwn.college using pipe(|)
- Command: /challenge/run | grep pwn.college
- Flag: pwn.college{sjDhZZPjgxAolPM2K3LWZMca1FO.dlTM4QDLxIjN0czW}
### Grepping errors
- Process: first redirect standard error to standard output using 2>&1 and then grep pwn
- Command: /challenge/run 2>&1 | grep pwn.college
- Flag: pwn.college{AbMxsVApHr8PH6EVTFDAGuaGW1U.dVDM5QDLxIjN0czW}
### Duplicating piped data with tee
- Process: tee the copy of pwn to different file and then cat the file to get secret code and then execute both the command
- Command: /challenge/pwn | tee cmd_1 | /challenge/college , cat cmd_1 , /challenge/pwn --secret EBtwsM9L | /challenge/college
- Flag: pwn.college{EBtwsM9LZBKzGXjEV4RcIRzu0VO.dFjM5QDLxIjN0czW}
### Writing to multiple programs
- Process: Duplicate the data to give input in two files using tee >()
- Command: /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
- Flag: pwn.college{0Cm-Vn8O_fNxoQvF5tk46fyeHcG.dBDO0UDLxIjN0czW}
### Split-piping stderr and stdout
- Process: Send stderr to /challenge/the and stdout to /challenge/planet from /challenge/hack
- Command: /challenge/hack > >(/challenge/planet) 2> >(/challenge/the) 
- Flag: pwn.college{wybE1ta_AiCynJlO2loLYAg75yq.dFDNwYDLxIjN0czW}
