# nmap

**Common Commands**

- Nmap --version to check the version of nmap
- sudo apt update nmap to update nmap if needed  
- Man nmap to access manual for nmap
- Nmap --help to get help with nmap commands

**Performing nmap scan**

- You can notice the number of open ports and what servies they run
 ○ Here is how to run an nmap scan nmap scanme.nmap.org.
 ○ To run a nmap in your subnet network /30 we use nmap scanm.nmap.org/30

- Scanning on a target ip nmap 'targetip'
    - Ex: nmap  172.0.0.1
        - ![alt text](<img/nmap 127.0.0.1.png>)

- Performing a nmap scan using specific options 
    - Running a nmap scan using options to further assess the network. 
        - Nmap -A  -T4 target/host 
        - ![](<img/nmap -A -T.png>)

- Output Nmap Scan Results to a File 
    - Performing a scan on a target who is on the network and outputs the scan    results into a file.
        - Change directory to a directory where you want to save your scan results using "cd #path_of_your_directory".
            -  -p option to scan a specific port. 
            - -oN to output our results to a scan.txt.
            - -A to run an aggressive scan and retrieve information about OS detection, version detection and script scanning. 
            - ![](<img/nmap 127.0.0.1.png>)

 _Note_  - When the service "tcpwrapped" is displayed it means that the port is being controlled by a tcpwrapper which is a software solution that provides additionally firewall features. The tcp wrapper monitors all incoming packets and checks if the node is attempting to connect is authorized based on various criteria specified  
