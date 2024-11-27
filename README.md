<h1>PowerShell</h1>

<h2>Description</h2>
Project consists of simulating a workplace environment by creating 1000+ new users using PowerShell. 
<br />


<h2>Languages and VM Platform</h2>

- <b>PowerShell</b> 
- <b>VirtualBox</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Script walk-through & Explanation:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://imgur.com/RwjV3L3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Utilized Script:  <br/>
<img src="https://imgur.com/76QG10U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
All users will use "Password1" as Password: <br/>
<img src="https://imgur.com/PFVdM6Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Utilize auto-generated names in file "names.txt. to created user list:  <br/>
<img src="https://imgur.com/3CiROsg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
"ConvertTo-SecureString" converts the plain text password users input (Password1) into an "object" PowerShell can use during user creation:  <br/>
<img src="https://imgur.com/6lmvSmw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creates a new "folder" in active directory Called USERS, unticks prevent accidental deletion box:  <br/>
<img src="https://imgur.com/A6ygND7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Loop: will run following code for all new users accounts created:  <br/>
<img src="https://imgur.com/OHkk1Fm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Splits the full name into first(name) and last(surname):  <br/>
<img src="https://imgur.com/laJAB2r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<br />
Takes first character on first(name) adds it to last(surname) in lowercase:  <br/>
<img src="https://imgur.com/rZsG0qX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<br />
Creates new users in active directory: <br/>
<img src="https://imgur.com/EYKtigq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Execute script and check new users: <br/>
<img src="https://imgur.com/jm1f1lm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
