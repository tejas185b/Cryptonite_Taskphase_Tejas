## SHELL VARIABLES
### Printing variables
- Command: echo $FLAG
- Flag: pwn.college{caI46YCBEBbemrXYXZVSMMm7SO3.ddTN1QDLxIjN0czW}
### Setting variables
- Command: PWN=COLLEGE
- Flag: pwn.college{wLeOqsjHiiMWAYZR_ybbEItUjBX.dlTN1QDLxIjN0czW}
### Multi-word variables
- Command: PWN="COLLEGE YEAH"
- Flag: pwn.college{w60J1BvX4TZY48_yETp10XzcZ_y.dBjN1QDLxIjN0czW}
### Exporting variables
- Command: export PWN=COLLEGE , COLLEGE=PWN , /challenge/run
- Flag: pwn.college{MZ3sbeBD69EulIiaMrhpGZp9J0_.dJjN1QDLxIjN0czW}
### Printing exported variables
- Command: env
- Flag:  pwn.college{sIFArSp_lCaxPTxbqw9P2Agjw9h.dhTN1QDLxIjN0czW}
### Storing command output
- Command: PWN=$(/challenge/run) , echo $PWN
- Flag: pwn.college{kaQr4MaZ7b32CQruFG0FaUNHfbT.dVzN0UDLxIjN0czW}
### Reading input
- Command: read PWN
- Flag: pwn.college{oye0kUgo1MrmqJX0FAi-rg-0xdB.dhzN1QDLxIjN0czW
### Reading files
- Command: read PWN < /challenge/read_me
- Flag: pwn.college{0aGzBl5kRWv6Cge7VY6CxUEN12G.dBjM4QDLxIjN0czW}
## PROCESSES AND JOBS
### Listing processes
- Command: ps -ef , /challenge/1153-run-14617
- Flag:  pwn.college{EbuReluF-syFXISLhZJsPKy1Ie8.dhzM4QDLxIjN0czW}
### Killing processes
- Command: ps -ef , kill 73 , /challenge/run
- Flag: pwn.college{wGH4QMa1Uph0fzquo-LMflw17fJ.dJDN4QDLxIjN0czW}
### Interrupting processes
- Command: /challenge/run , (ctrl +  c)
- Flag: pwn.college{QrsODqa2pP3hp283u1W-jxESeFk.dNDN4QDLxIjN0czW}
### Suspending processes
- Command: /challenge/run , (ctrl + z) , /challenge/run
- Flag: pwn.college{8NMyje8DhkG_Y8EvtfHx8WeO_Ig.dVDN4QDLxIjN0czW}
### Resuming processes
- Command: /challenge/run , (ctrl + z) , fg
- Flag: pwn.college{cn2Ppeh4R_dQyHkp5BA-iMqHQRh.dZDN4QDLxIjN0czW}
### Backgrounding processes
- Command: /challenge/run , (ctrl + z) , bg , /challenge/run
- Flag: pwn.college{8_VZmSyLxAvdeFPOe02EliRrAg9.ddDN4QDLxIjN0czW}
### Foregrounding processes
- Command:  /challenge/run , (ctrl + z) , bg , fg
- Flag: pwn.college{8Ziieir3jXMnZmusUh3T1K3znfi.dhDN4QDLxIjN0czW}
### Starting backgrounded process
- Command: /challenge/run &
- Flag: pwn.college{kUD57J31tfQtmuH_-2zuV3YhZEd.dlDN4QDLxIjN0czW}
### Process exit codes
- Command: /challenge/get-code $? , /challenge/submit-code $?
- Flag: pwn.college{s6qkTW4CGFBLwPACJfC7LTazf7G.dljN4UDLxIjN0czW}
## PERCIEVING PERMISSIONS
### Changing file ownership
- Command: chown hacker /flag , cat /flag
- Flag: pwn.college{4PAPoM3F-YckWCtxIBu5oDXSH3N.dFTM2QDLxIjN0czW}
### Groups and files
- Command: chgrp hacker /flag , cat /flag
- Flag: pwn.college{8WvasBKAD_Jr9_GljanlPDgRMJI.dFzNyUDLxIjN0czW}
### Fun with group names
- Command: id , chgrp group6417 /flag , cat /flag
- Flag: pwn.college{wxYtqatkkvGGdgwKXeSqSfEdGYq.dJzNyUDLxIjN0czW}
### Changing permissions
- Command: chmod go+r /flag , cat /flag
- Flag: pwn.college{spIpumjd5fDK0TFgjqanK-aET_8.dNzNyUDLxIjN0czW}
### Executable files
- Command: chmod o+x /challenge/run , challenge/run
- Flag: pwn.college{Q6GfO5jIWZ8TIiA0-b6Eo56SNpn.dJTM2QDLxIjN0czW}
### Permission tweaking process
- Command:  keep using chmod and editing permissions of /challenge/pwn file 8 times then use chmod ugo+rwx /flag
- Flag: pwn.college{8bvReg4HNWYeR65l_Mn9VDPRY3L.dBTM2QDLxIjN0czW}
### Permissions setting practice
- Command: keep using chmod and editing permissions of /challenge/pwn file 8 times using chaining and = then use chmod a=rwx /flag
- Flag: pwn.college{gKcf7B-e9VHKDerpFlAHipe1Nxs.dNTM5QDLxIjN0czW}
### The SUID bit
- Command: chmod u+s /challenge/getroot ,  /challenge/getroot , cat /flag
- Flag: pwn.college{ghG1tA9A-z-bSzR6xXbTZhof4NQ.dNTM2QDLxIjN0czW}
## UNTANGLING USERS
### Becoming root with su
-	Command: su , enter pwd “hack-the-planet” ,  cat /flag
-	Flag: pwn.college{A4MB3uKRTq_Di23ZJjuU_a1kMpw.dVTN0UDLxIjN0czW}
### Other users with su
-	Command: su zardus , , enter pwd “dont-hack-me” , /challenge/run  
-	Flag: pwn.college{MN8niRIiv5jg-8O75mTU2MMEodW.dZTN0UDLxIjN0czW}
### Cracking passwords
-	Command:  john /challenge/shadow-leak , su zardus , enter pwd “aardvark” , /challenge/run
-	Flag: pwn.college{Io3LdmIqzXizDtHHsZa73k5PQqs.ddTN0UDLxIjN0czW}
### Using sudo
-	Command: sudo cat /flag
-	Flag: pwn.college{Ap0DHFQQKlCa-gJnYe2w4KOL8Sw.dhTN0UDLxIjN0czW}
## CHAINING COMMANDS
### Chaining with semicolons
-	Command: /challenge/pwn; /challenge/college
-	Flag: pwn.college{M7oiudnywJHKecgY5eSd2_AmrZr.dVTN4QDLxIjN0czW}
### Your first shell script
-	Command: nano x.sh , write in file “/challenge/pwn; /challenge/college” , bash x.sh
-	Flag: pwn.college{srLMhgCnH4RFnk63Fv30lIRwbFc.dFzN4QDLxIjN0czW}
### Redirecting script output
-	Command: nano x.sh , write in file “/challenge/pwn; /challenge/college” , bash x.sh | /challenge solve
-	Flag: pwn.college{QUTL5797pvxzpe1FEJFCc2Ok1UK.dhTM5QDLxIjN0czW}
### Executable shell scripts 
-	Command: nano x.sh , write “/challenge/solve” , chmod a=rwx x.sh , ./x.sh
-	Flag: pwn.college{MO339oA3fTa_XBjA-BkyuD7O-KV.dRzNyUDLxIjN0czW}
## PONDERING PATH
### The PATH variable
-	Command: PATH="" , /challenge/run
-	Flag: pwn.college{Asw1ni5HhWwp2dtXg_YZvJ6NbYK.dZzNwUDLxIjN0czW}
### Setting PATH
-	Command: PATH="/challenge/more_commands" , /challenge/run
-	Flag: pwn.college{IAEvDa7BCVC3OO0lEX5mj0oWRDW.dVzNyUDLxIjN0czW}
### Adding commands
-	Command: find / -name cat , nano win , write “/usr/bin/cat /flag” in win , PATH="/home/hacker:$PATH" , chmod +x win , /challenge/run
-	Flag:  pwn.college{0Tqzeai9wmbk0CozKG37hrkH9OM.dZzNyUDLxIjN0czW}
### Hijacking commands
-	Command: nano rm , write “/usr/bin/cat /flag” in rm , PATH="/home/hacker" , chmod +x rm , /challenge/run
-	Flag: pwn.college{kYV6lrJZh8fZ2lOU9kze5mzRYg6.ddzNyUDLxIjN0czW}



