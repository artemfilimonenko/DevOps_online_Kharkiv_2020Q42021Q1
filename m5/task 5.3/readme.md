   #     Module 5. Linux Essentials
   ##    Task 5.3
   ###   Part 1

  1. Processes in Linux have the following states:

  <img src=".\screenshots 5.3\111.png" width="55%"/>
  
  2. pstree shows the running processes as a tree
  
  <img src=".\screenshots 5.3\1.pstree.png" width="55%"/>
  
  3. proc is a virtual filesystem. It contains runtime system information (e.g. system memory, devices mounted, hardware configuration, etc). 
     It can be regarded as a control and information centre for the kernel.
  
  4. Printed information about the processor

  <img src=".\screenshots 5.3\2.cat cpuinfo.png" width="55%"/>
  
  5. *"Use the ps command to get information about the process. The information should be as
follows: the owner of the process, the arguments with which the process was launched for
execution, the group owner of this process, etc"*

  <img src=".\screenshots 5.3\3.ps command.png" width="55%"/>
  
  6. *"How to define kernel processes and user processes?"* - execute ps and check PID
 
  7. ps aux 

  <img src=".\screenshots 5.3\4.ps aux, describing processes status.png" width="55%"/>
  
  8. *Display only the processes of a specific user*
  
  <img src=".\screenshots 5.3\5.ps -u artem.png" width="55%"/>
  
  9. Top is an utility that shows the states of processes and their realtime activity.
   
  <img src=".\screenshots 5.3\6.top info.png" width="55%"/>
  
  10. top -u root

  <img src=".\screenshots 5.3\7.top -u root.png" width="55%"/>

  11. *"What interactive commands can be used to control the top command? Give a couple of examples."*
        space - refresh the screen;
        k - kill a process;
        Shift + P - sort by CPU load
        
  12. Sorting processes by CPU load
  
  <img src=".\screenshots 5.3\8.Shift + P.png" width="55%"/>
  
  13. nice and renice are commands to set the process priority. 
  14. There is an opportunity to change process priority via top by clicking *r*
  15.  The kill command is used to send a signal to a process. By default if we do not specify which signal to send, the SIGTERM signal is sent.
  SIGTERM tells the process to exit. Each signal has its own number. SIGTERM is numbered 15. 
  A list of all signals (and their numbers) that the kill command can send can be displayed by executing kill -l.
  The following command is used to send a signal: kill –s signal pid.
  The -9 signal is used to force termination.
  
  <img src=".\screenshots 5.3\9.kill -l.png" width="55%"/>

  16. 

    jobs - shows current jobs;
    bg - run a job in the background, until you closed a shell;
    fg - run it in the foreground;
    nohup - run a job in the background, even after you closed a shell or even logout;
    
  <img src=".\screenshots 5.3\11. sleep bg fg nohup_1.png" width="55%"/>

  <img src=".\screenshots 5.3\12.sleep bg fg nohup_2png" width="55%"/>

  ### Part 2
  
  1. Checking if OpenSSH services being installed

  <img src=".\screenshots 5.3\13.windcapability.jpg" width="55%"/>
  
  2. Checking the implementability of the most frequently used OPENSSH commands in the MS Windows operating system.
     ssh, ssh-keygen, scp

  <img src=".\screenshots 5.3\14.sshcommand.jpg" width="55%"/>

  <img src=".\screenshots 5.3\15.ssh-keygencommand.jpg" width="55%"/>

  <img src=".\screenshots 5.3\16.scp command.jpg" width="55%"/>

  3. Implementing basic SSH settings to increase the security of the client-server connection via editing sshd_config

  <img src=".\screenshots 5.3\17.rootlogin-no.png" width="55%"/>

  <img src=".\screenshots 5.3\18.passauthentication.png" width="55%"/>

  <img src=".\screenshots 5.3\19.Changed port.png" width="55%"/>

  4. Different options for encryption keys in SSH (rsa, ecdsa, ed25519)

  <img src=".\screenshots 5.3\20.rsa 1024.png" width="55%"/>

  <img src=".\screenshots 5.3\21.ecdsa.png" width="55%"/>

  <img src=".\screenshots 5.3\22.ed25519.png" width="55%"/>

  5. Implementing port forwarding for the SSH client in VirtualBox
 
  <img src=".\screenshots 5.3\23.portforwarding1.jpg" width="55%"/>

  <img src=".\screenshots 5.3\24.portforwarding2.jpg" width="55%"/>
