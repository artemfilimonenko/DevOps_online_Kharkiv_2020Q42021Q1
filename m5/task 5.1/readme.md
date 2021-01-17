<html>
  <body>
    <h1>Module 5</h1>
    <h2>Linux Essentials</h2>
    <h3>Task 5.1</h3>

<h4><em>Part 1</em></h4>

1. Established SSH connection using MobaXterm as a client (logged via pass)

<img src=".\screenshots 5.1\part 1\1.ssh_establishing.jpg" width="75%"/>

2. Logged as root, changed password through 'passwd' command . *What system file does it change?* - /etc/shadow

<img src=".\screenshots 5.1\part 1\2.login as root and passwd.jpg" width="75%"/>

3. In order to see all the users registered in system I used command: "cat /etc/passwd". We might glean such information about user:<br>
login : password : UID : GID : GECOS : home : shell

<img src=".\screenshots 5.1\part 1\3.etc passwd.jpg" width="75%"/>

4. Changed personal info via "chfn" command

<img src=".\screenshots 5.1\part 1\4.chfn.jpg" width="75%"/>

5. Got acquainted with 'man' and 'info'. Practiced with both commands using different keys.

<img src=".\screenshots 5.1\part 1\5.Man_info.jpg" width="75%"/>

6. Explored 'more' and 'less' commands. Viewed content of .bashrc (using 'more') and .bash_history (using 'less')

<img src=".\screenshots 5.1\part 1\6.More.jpg" width="75%"/>
<img src=".\screenshots 5.1\part 1\7.Less.jpg" width="75%"/>

7. Changed .plan file. Let's check what information 'finger' cosists of:

<img src=".\screenshots 5.1\part 1\8.changing plan.jpg" width="75%"/>

8. Listed home directory

<img src=".\screenshots 5.1\part 1\9.ls command.jpg" width="75%"/>


<h4><em>Part 2</em></h4>


1. Became familiar with 'tree' command. 

<img src=".\screenshots 5.1\part 2\1.man_tree.jpg" width="75%"/>

1.1. Output all files that contain symbol "c"

<img src=".\screenshots 5.1/part 2/2.Tree output.jpg" width="75%"/>

1.2. Output all files that contain following sequence of characters: "ctl"

<img src=".\screenshots 5.1/part 2/2.Tree output_2.jpg" width="75%"/>

1.2.3 List subdirectories of the root directory up to and including the second nesting level

<img src=".\screenshots 5.1\part 2\3.tree -L 2.jpg" width="75%"/>
2. Type of file determination 

<img src=".\screenshots 5.1\part 2\4.file type.jpg" width="75%"/>

3. 'cd ../..' allows to go back to your home directory from anywhere in the filesystem

<img src=".\screenshots 5.1\part 2\5.cd .....jpg" width="75%"/>

4. Examined 'ls' command and its parameters: -l, -a
<br> '-a' - <em>In directories, do not ignore file names that start with ‘.’</em> </br>
<br> '-l' - print the file type, file mode bits, number of hard links, owner name etc.</br>

<img src=".\screenshots 5.1\part 2\6.ls -l ls -a.jpg" width="75%"/>

5. The task contained the following steps:<br>
- create a subdirectory in the home directory<br>
- in this subdirectory create a file containing information about directories located in the root directory (using I/O redirection operations);<br>
- view the created file;<br>
- copy the created file to your home directory using relative and absolute addressing.<br>
- delete the previously created subdirectory with the file requesting removal;<br>
- delete the file copied to the home directory.</br>

<img src=".\screenshots 5.1\part 2\7.jpg" width="75%"/>
<img src=".\screenshots 5.1\part 2\8.jpg" width="75%"/>

6. Performed the following sequence of operations

- Created a subdirectory "test" in the home directory;<br>
- Copied the .bash_history file to this directory while changing its name to "labwork2";<br>
- Create a hard and soft link to the labwork2 file in the test subdirectory;<br> 
- Renamed the hard link file to hard_lnk_labwork2;<br> 
- Renamed the soft link file to symb_lnk_labwork2;<br> 
- Deleted the labwork2. <em>Symb link is null now.</em></br>

<img src=".\screenshots 5.1\part 2\8..jpg" width="75%"/>
<img src=".\screenshots 5.1\part 2\10.jpg" width="75%"/>

7.Found all files that containt "squid" and "traceroute" using 'locate'

<img src=".\screenshots 5.1\part 2\11.Locate.jpg" width="75%"/>

8. Mounted partitions determination

<img src=".\screenshots 5.1\part 2\12.df -h.jpg" width="75%"/>

9. <em>Count the number of lines containing a given sequence of characters in a given file.</em>

<img src=".\screenshots 5.1\part 2\13..jpg" width="75%"/>

10. Found all files in the /etc directory that contain "host" character sequence.

<img src=".\screenshots 5.1\part 2\14.jpg" width="75%"/>

11. <em>List all objects in /etc that contain the ss character sequence. How can I duplicate a similar command using a bunch of grep?</em>

<img src=".\screenshots 5.1\part 2\15.jpg" width="75%"/>

12. <em>Organize a screen-by-screen print of the contents of the /etc directory.</em>

<img src=".\screenshots 5.1\part 2\16.jpg" width="75%"/>

13. <em>List the first 5 directory files that were recently accessed in the /etc directory</em>

<img src=".\screenshots 5.1\part 2\18.jpg" width="75%"/>

</body>
</html>
