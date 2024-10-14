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



