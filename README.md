# Work-Through-
**STEP 1:** Scaning  server for open port using the following command “sudo -sS nmap 172.16.0.3”. The screenshot below shows the open port (8021) indicated with red arrow which can be a suitable target.  
![image](https://github.com/Mirian02/Work-Through-/assets/118598344/cc5be323-f440-4bb4-a6ad-66592d9c81c3)

**STEP 2:** In kali, metaspoilt was utilized by the actor to carry out the DoS attack. Metaspoilt has this auxiliary called SynFlood, the actor will be using that SynFlood to attack the target machine. In other to run metaspoilt “sudo msfconsole” command is used, after using “pwd” to locate the file folder. From the below screenshot (highlighted in yellow), it shows Metaspoilt has about 1062 auxxiliary and the actor is looking for the one which is “SynFlood”.
![image](https://github.com/Mirian02/Work-Through-/assets/118598344/5893d0f9-6fd0-4a0b-8af5-a8a562a3fad8)

**STEP 3:** command “search synflood” is used to search for the location of the exact auxiliary needed. Below screenshots displays the location.
![image](https://github.com/Mirian02/Work-Through-/assets/118598344/8f66a702-7cea-45fd-8458-1b9614e3d109)

**STEP 4:** The screenshots below “shows options” of the interface (a name can be given to the interface machine but it is not required), number ( the actor can have numbers of the packet which is being sent but is not required), RHOST (R host is the remote host (victim machine), the host needs to be set to the location the actor wants to attack), from the diagram the remote port has picked up 80 by default but the hacker will be using port 8021 which was seen earlier when checking for open port and the SHOST which will be the ip address of the attacker machine (host machine). 
<img width="379" alt="image" src="https://github.com/Mirian02/Work-Through-/assets/118598344/de031d4d-9441-4109-be8f-7e6d993d9f91">

**STEP 5:** Setting the target remote HOST (windows), remote PORT, Spoof IP address and show options.
<img width="356" alt="image" src="https://github.com/Mirian02/Work-Through-/assets/118598344/f96124c2-06f7-4179-a2bb-5c36e38c7dca">

**STEP 6: **Command “exploit” to recieve traffic, below screenshots shows the SYN flooding. 
<img width="415" alt="image" src="https://github.com/Mirian02/Work-Through-/assets/118598344/170f494e-f8e9-4109-bfaf-5ceeb285bcc0">

Step 7: the actor loads wireshack in other to see the amount of traffic is receiving from the target machine as shown in the below screentshot.
<img width="468" alt="image" src="https://github.com/Mirian02/Work-Through-/assets/118598344/5506ea94-4149-4f29-ac26-b2a7bbc31ee2">


