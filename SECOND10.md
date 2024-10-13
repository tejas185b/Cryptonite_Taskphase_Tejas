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

