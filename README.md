# Work-Through-
DENIAL OF SERVICE (Using SynFlood) ATTACK 
When two notes are trying to communicate, they may use a THREE WAY HANDSHAKE, the actor will be using a target and attacking machine, the attacking machine will be sending a SYN packet and if the packet goes to the target machine, the target machine will reply with an acknowledgement (SYN/ACK) packet. After that the target machine will be waiting to get the final package from source again which will be ACK packets. The actor will load the target machine with many task and with that it will cause DoS. 
Metaspoilt in kali VM will be used as the attacking maching while centos will be used as the target machine. 

**STEP 1:** Scaning  server for open port using the following command “sudo -sS nmap 172.16.0.3”. The screenshot below shows the open port (8021) indicated with red arrow which can be a suitable target.  


![image](https://github.com/Mirian02/Work-Through-/assets/118598344/cc5be323-f440-4bb4-a6ad-66592d9c81c3)
STEP 2: In kali, metaspoilt was utilized by the actor to carry out the DoS attack. Metaspoilt has this auxiliary called SynFlood, the actor will be using that SynFlood to attack the target machine. In other to run metaspoilt “sudo msfconsole” command is used, after using “pwd” to locate the file folder. From the below screenshot (highlighted in yellow), it shows Metaspoilt has about 1062 auxxiliary and the actor is looking for the one which is “SynFlood”.


![image](https://github.com/Mirian02/Work-Through-/assets/118598344/5893d0f9-6fd0-4a0b-8af5-a8a562a3fad8)
