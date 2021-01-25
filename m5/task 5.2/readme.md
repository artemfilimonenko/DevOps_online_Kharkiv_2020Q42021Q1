<html>
  <body>
    <h1>Module 5</h1>
    <h2>Linux Essentials</h2>
    <h3>Task 5.2</h3>

1. Established SSH connection using key-based authentication

<img src=".\screenshots 5.2\1.ssh establishing .png" width="55%"/>

2. /etc/passwd file is a colon-separated file that contains the following information:<br>
 - User name<br>
- Encrypted password<br>
- User ID number (UID)<br>
- User's group ID number (GID)<br>
- Full name of the user (GECOS)<br>
- User home directory<br>
- Login shell<br>

<img src=".\screenshots 5.2\2.etc passwd.png" width="55%"/>

/etc/group file contains basic group attributes.Each record appears on a single line and is the following format:<br>
Name:Password:ID:User1,User2,...,Usern<br>

<img src=".\screenshots 5.2\3.etc group.png" width="55%"/>

There are such types of user:<br>
- root;<br>
- pseudo-users;<br>
- service users;<br>
- regular users.<br>

Examples of pseudo-users:
- daemon;
- adm;
- uucp.<br>

We can define them via UID.

3. UID is a unique number assigned to a given user.<br>
UID ranges:<br>
- 0 - root;
- 1-10 - pseudo-users;
- 11-99 - service users;
- 100+ - regular users.<br>

In order to define UID we can use command id or check <em>passwd</em> file<br>

<img src=".\screenshots 5.2\4.UID.png" width="55%"/>

4. GID is a value used to represent a specific group<br>

<img src=".\screenshots 5.2\5.GID.png" width="55%"/>

5. To determine belonging of user to the specific group we need to check <em>/etc/groups</em> file.<br>

6.There are two commands to creating a user: useradd, adduser.<br>
Basic parameters required to create a user:<br>
- username;
- password;
- assign a group.<br> 

<img src=".\screenshots 5.2\6.adduser useradd.png" width="55%"/>

7. In order to change account name we can use usermod -l command<br>

<img src=".\screenshots 5.2\7.usermod -l.png" width="55%"/>

8. /etc/skel is a template of home directory.<br>
It contains files and directories that are automatically copied over to a new user's when it is created from useradd command.<br>

9. <em>How to remove a user from the system (including his mailbox)?</em>  userdel -r<br>

<img src=".\screenshots 5.2\8.uderdel -r.png" width="55%"/>

10. To lock/unlock user account should be used passwd command with keys -l -u

<img src=".\screenshots 5.2\9.lock and  unlock user.png" width="55%"/>

11. <em>How to remove a user's password and provide him with a password-free login for subsequent password change?</em> passwd -d<br>

<img src=".\screenshots 5.2\10.passwd -d .png" width="55%"/>

12. ls -al allows to display extended format of information about the directory<br>

<img src=".\screenshots 5.2\11.directory extended info.png" width="55%"/>

Information columns:<br>
- file type;<br>
- permissions for user (read; write; execute);<br>
- access rights for groups (read; write; execute);<br>
- access rights for others (read; write; execute);<br> 
- amount of hard links;<br> 
- user identifier;<br> 
- username;<br> 
- group ID;<br> 
- last modification date;<br> 
- file/dir name.<br>

13. <em>What access rights exist and for whom (i. e., describe the main roles)? Briefly describe the acronym for access rights.</em><br>
There are three types of useres related to the file permissions:<br>
- owner;<br>
- group;<br>
- others.<br>

Permission types:<br>
- read; it is denoted by ‘r’ when it is defined by character, and it is denoted by 4 when it is defined by a number;<br>
- write; it is denoted by ‘w’ when it is defined by character, and it is denoted by 2 when it is defined by a number;<br>
- execute; it is denoted by ‘x’ when it is defined by character, and it is denoted by 1 when it is defined by a number.<br>

14.If the file's UID  matches the process UID then user is the owner of the file.<br>
If file's GID matches the GID of any group, that the user is a member of the group that the file belongs. 
If neither the UID nor the GID of the file intersect with UID of the process and a list of groups that started the user, this user is an outsider.<br>

15. In order to change file owner uses command <em>chown</em>. To change permissions uses command <em>chmod</em>.

<img src=".\screenshots 5.2\12.chown.png" width="55%"/>
<img src=".\screenshots 5.2\13.chmod.png" width="55%"/>

16. Here below a table of octal representation of access rights<br>

<img src=".\screenshots 5.2\20.png" width="55%"/>

An example:<br>
<img src=".\screenshots 5.2\14.file permissions (octal).png" width="55%"/>

<em>umask</em> is an utility that allows you to view or to set the file mode creation mask, which determines the permissions bits for newly created files or directories.<br>
Changing <em>umask</em>

<img src=".\screenshots 5.2\15.umask.png" width="55%"/>

17. Sticky bit sets for a folder/file so only the file's/folder's owner or root user can rename or delete the file.

<img src=".\screenshots 5.2\16.chmod sticky bit.png" width="55%"/>

18. Command script should have permission for execution, also read,write permissions if it's needed.

<img src=".\screenshots 5.2\17.file attributes for executing.png" width="55%"/>
