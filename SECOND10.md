## SHELL VARIABLES
### Printing variables
- Process: just echo the variable FLAG
- Command: echo $FLAG
- Flag: pwn.college{caI46YCBEBbemrXYXZVSMMm7SO3.ddTN1QDLxIjN0czW}
### Setting variables
- Process: set the value of variable PWN as COLLEGE
- Command: PWN=COLLEGE
- Flag: pwn.college{wLeOqsjHiiMWAYZR_ybbEItUjBX.dlTN1QDLxIjN0czW}
### Multi-word variables
- Process: Set the variable PWN as "COLLEGE YEAH"
- Command: PWN="COLLEGE YEAH"
- Flag: pwn.college{w60J1BvX4TZY48_yETp10XzcZ_y.dBjN1QDLxIjN0czW}
### Exporting variables
- Process: Set the value of COLLEGE to PWN and then export the variable PWN setting its value COLLEGE and then run /challenge/run passing the variable PWN
- Command: export PWN=COLLEGE , COLLEGE=PWN , /challenge/run
- Flag: pwn.college{MZ3sbeBD69EulIiaMrhpGZp9J0_.dJjN1QDLxIjN0czW}
### Printing exported variables
- Process: use env command to print all the exported variable set and grep the word FLAG
- Command: env
- Flag:  pwn.college{sIFArSp_lCaxPTxbqw9P2Agjw9h.dhTN1QDLxIjN0czW}
### Storing command output
- Process: Store the output as /challenge/run to PWN and then read it
- Command: PWN=$(/challenge/run) , echo $PWN
- Flag: pwn.college{kaQr4MaZ7b32CQruFG0FaUNHfbT.dVzN0UDLxIjN0czW}
### Reading input
- Process: use read command to set COLLEGE as the value of PWN
- Command: read PWN
- Flag: pwn.college{oye0kUgo1MrmqJX0FAi-rg-0xdB.dhzN1QDLxIjN0czW
### Reading files
- Process: use read command to set the value of variable PWN as output of /challenge/run
- Command: read PWN < /challenge/read_me
- Flag: pwn.college{0aGzBl5kRWv6Cge7VY6CxUEN12G.dBjM4QDLxIjN0czW}
## PROCESSES AND JOBS
### Listing processes
- Process: In this use ps command along with -ef to check if /challenge file is running
- Command: ps -ef , /challenge/1153-run-14617
- Flag:  pwn.college{EbuReluF-syFXISLhZJsPKy1Ie8.dhzM4QDLxIjN0czW}
### Killing processes
- Process: In this first find /challenge/run using the command ps -ef | grep /challenge/dont_run and then kill it
- Command: ps -ef , kill 73 , /challenge/run
- Flag: pwn.college{wGH4QMa1Uph0fzquo-LMflw17fJ.dJDN4QDLxIjN0czW}
### Interrupting processes
- Process: Interreput the process using ^C
- Command: /challenge/run , (ctrl +  c)
- Flag: pwn.college{QrsODqa2pP3hp283u1W-jxESeFk.dNDN4QDLxIjN0czW}
### Suspending processes
- Process: first run /challenge/run and then suspend it using ^Z and then again run it
- Command: /challenge/run , (ctrl + z) , /challenge/run
- Flag: pwn.college{8NMyje8DhkG_Y8EvtfHx8WeO_Ig.dVDN4QDLxIjN0czW}
### Resuming processes
- Process: first suspend the process usinf ^Z and then resume it using command fg
- Command: /challenge/run , (ctrl + z) , fg
- Flag: pwn.college{cn2Ppeh4R_dQyHkp5BA-iMqHQRh.dZDN4QDLxIjN0czW}
### Backgrounding processes
- Process: First 'run' and then suspend the process and then use command bg to run it in background and then make a copy of it
- Command: /challenge/run , (ctrl + z) , bg , /challenge/run
- Flag: pwn.college{8_VZmSyLxAvdeFPOe02EliRrAg9.ddDN4QDLxIjN0czW}
### Foregrounding processes
- Process: First suspend the process then background the process and then foreground the process
- Command:  /challenge/run , (ctrl + z) , bg , fg
- Flag: pwn.college{8Ziieir3jXMnZmusUh3T1K3znfi.dhDN4QDLxIjN0czW}
### Starting backgrounded process
- Process: background the process using &
- Command: /challenge/run &
- Flag: pwn.college{kUD57J31tfQtmuH_-2zuV3YhZEd.dlDN4QDLxIjN0czW}
### Process exit codes
- Process: first run /challenge/get-code which will give error and then read the error using $? and then pass the error to /challenge/submit-code
- Command: /challenge/get-code $? , /challenge/submit-code $?
- Flag: pwn.college{s6qkTW4CGFBLwPACJfC7LTazf7G.dljN4UDLxIjN0czW}
## PERCIEVING PERMISSIONS
### Changing file ownership
- Process: Change the owner of /flag to hacker using command chown and then read the file.
- Command: chown hacker /flag , cat /flag
- Flag: pwn.college{4PAPoM3F-YckWCtxIBu5oDXSH3N.dFTM2QDLxIjN0czW}
### Groups and files
- Process: Change the group to hacker for the file /flag using chgrp and then read the file.
- Command: chgrp hacker /flag , cat /flag
- Flag: pwn.college{8WvasBKAD_Jr9_GljanlPDgRMJI.dFzNyUDLxIjN0czW}
### Fun with group names
- Process: first use the id command to check which group the user belong to and then use chgrp command to /flag access to that group and then read it.
- Command: id , chgrp group6417 /flag , cat /flag
- Flag: pwn.college{wxYtqatkkvGGdgwKXeSqSfEdGYq.dJzNyUDLxIjN0czW}
### Changing permissions
- Process: change mode to other and give read access using chmod command
- Command: chmod go+r /flag , cat /flag
- Flag: pwn.college{spIpumjd5fDK0TFgjqanK-aET_8.dNzNyUDLxIjN0czW}
### Executable files
- Process: Change the access of execution of /challenge/run
- Command: chmod o+x /challenge/run , challenge/run
- Flag: pwn.college{Q6GfO5jIWZ8TIiA0-b6Eo56SNpn.dJTM2QDLxIjN0czW}
### Permission tweaking process
- Process: Change permissions accroding to the demands of the challenge
- Command:  keep using chmod and editing permissions of /challenge/pwn file 8 times then use chmod ugo+rwx /flag
- Flag: pwn.college{8bvReg4HNWYeR65l_Mn9VDPRY3L.dBTM2QDLxIjN0czW}
### Permissions setting practice
- Process: Change permissions accroding to the demands of the challenge using = and , .
- Command: keep using chmod and editing permissions of /challenge/pwn file 8 times using chaining and = then use chmod a=rwx /flag
- Flag: pwn.college{gKcf7B-e9VHKDerpFlAHipe1Nxs.dNTM5QDLxIjN0czW}
### The SUID bit
- Process: Execute the file /challenge/getroot as root for that set the file as SUID bit using the command chmod u+s /challenge/getroot
- Command: chmod u+s /challenge/getroot ,  /challenge/getroot , cat /flag
- Flag: pwn.college{ghG1tA9A-z-bSzR6xXbTZhof4NQ.dNTM2QDLxIjN0czW}
## UNTANGLING USERS
### Becoming root with su
- Process: Become the root using su command and providing root password and then read flag
-	Command: su , enter pwd “hack-the-planet” ,  cat /flag
-	Flag: pwn.college{A4MB3uKRTq_Di23ZJjuU_a1kMpw.dVTN0UDLxIjN0czW}
### Other users with su
- Process: Become zardus user by passing it as argument to su command and then provide the password to access it and then execute /challenge/run
-	Command: su zardus , , enter pwd “dont-hack-me” , /challenge/run  
-	Flag: pwn.college{MN8niRIiv5jg-8O75mTU2MMEodW.dZTN0UDLxIjN0czW}
### Cracking passwords
- Process: Use john command on /challenge/shadow-leak which is the leaked file of /etc/shadow to decrypt the data and give a password and then use that password to access zardus user to run /challenge/run
-	Command:  john /challenge/shadow-leak , su zardus , enter pwd “aardvark” , /challenge/run
-	Flag: pwn.college{Io3LdmIqzXizDtHHsZa73k5PQqs.ddTN0UDLxIjN0czW}
### Using sudo
- Process: Use sudo command to read the flag as root as root has access to it.
-	Command: sudo cat /flag
-	Flag: pwn.college{Ap0DHFQQKlCa-gJnYe2w4KOL8Sw.dhTN0UDLxIjN0czW}
## CHAINING COMMANDS
### Chaining with semicolons
- Process: Enter the first command followed by ; and then the second command which will execute both the commands
-	Command: /challenge/pwn; /challenge/college
-	Flag: pwn.college{M7oiudnywJHKecgY5eSd2_AmrZr.dVTN4QDLxIjN0czW}
### Your first shell script
- Process: Using nano write the commands in x.sh file and then pass the x.sh file as argument to bash
-	Command: nano x.sh , write in file “/challenge/pwn; /challenge/college” , bash x.sh
-	Flag: pwn.college{srLMhgCnH4RFnk63Fv30lIRwbFc.dFzN4QDLxIjN0czW}
### Redirecting script output
- Process: create a .sh file with commands /challenge/pwn and /challenge/college and then pipe the output to /challenge/solve
-	Command: nano x.sh , write in file “/challenge/pwn; /challenge/college” , bash x.sh | /challenge solve
-	Flag: pwn.college{QUTL5797pvxzpe1FEJFCc2Ok1UK.dhTM5QDLxIjN0czW}
### Executable shell scripts 
- Process: Create a .sh file with command /challenge/solve and then make the .sh file executable using chmod command and then execute it.
-	Command: nano x.sh , write “/challenge/solve” , chmod a=rwx x.sh , ./x.sh
-	Flag: pwn.college{MO339oA3fTa_XBjA-BkyuD7O-KV.dRzNyUDLxIjN0czW}
## PONDERING PATH
### The PATH variable
- Process: set the PATH="" which will cause rm command to be lost therby executing the file without deleting its contents.
-	Command: PATH="" , /challenge/run
-	Flag: pwn.college{Asw1ni5HhWwp2dtXg_YZvJ6NbYK.dZzNwUDLxIjN0czW}
### Setting PATH
- Process: set the PATH=/challenge/more_commands/ to find the file and then run /challenge/run
-	Command: PATH="/challenge/more_commands" , /challenge/run
-	Flag: pwn.college{IAEvDa7BCVC3OO0lEX5mj0oWRDW.dVzNyUDLxIjN0czW}
### Adding commands
- Process: first find cat command directory using find / -name cat and then create win and inside the file write "usr/bin/cat /flag" and make it a executable file using chmod. After this change the PATH to /home/hacker and then run /challenge/run
-	Command: find / -name cat , nano win , write “/usr/bin/cat /flag” in win , PATH="/home/hacker:$PATH" , chmod +x win , /challenge/run
-	Flag:  pwn.college{0Tqzeai9wmbk0CozKG37hrkH9OM.dZzNyUDLxIjN0czW}
### Hijacking commands
- Process: we will create our own rm executable command which will read /flag so to access cat we will find path of cat and then write the rm file in /home/hacker to read flag. After this will make rm a executable file and then set the PATH to /home/hacker. If we then run /challenge/run we will get the flag.
-	Command: nano rm , write “/usr/bin/cat /flag” in rm , PATH="/home/hacker" , chmod +x rm , /challenge/run
-	Flag: pwn.college{kYV6lrJZh8fZ2lOU9kze5mzRYg6.ddzNyUDLxIjN0czW}



