# Simple SQL attack simulation and analysis


## Objective



### Skills Learned
- Understanding basic system enumeration 
- Practicing initial foothold techniques 
- Learning privilege escalation 
- Documenting attack methodology 
- Building confidence in ethical hacking 

### Tools Used


- Nmap -helped to identify th open ports,and running services like telnet.
- Telnet -used to connect on the targeted system (meowPC)
- kalilinux -used as the attacker PC
- openVPN -used to connect to the hack the box lab environment

## Steps

### Step 1 -connet to the HTB network via openvpn
![openvpn](https://github.com/user-attachments/assets/e5ad1ede-d6b1-4265-98c0-21c910a71d7a)

### Step 2-verify connectivity
![ping](https://github.com/user-attachments/assets/7cf3a81c-498f-4005-8bf1-66be714f3b4a)

### Step 3-Enumerate the Target
![nmap](https://github.com/user-attachments/assets/2ed55376-7f11-4988-a2d3-ceaf85a3a087)

### step 4-Exploit Telnet
![telnet](https://github.com/user-attachments/assets/e91f25dd-4ba6-473f-a580-eaf8e65274bc)
![telnet2](https://github.com/user-attachments/assets/4ea2ef91-993b-46ff-b7bc-fc5dd8623a7b)
- someimes, due to the configuration mistakes, some important accounts can be left with blanks passwords. So we can try some typical names such as admin, root, administrator etc.


### Step 5-Capture the flag
![flag](https://github.com/user-attachments/assets/2cd94e9f-299e-40ea-abc4-275d8329506a)



