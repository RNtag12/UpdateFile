<h1>File Update Through A Python Algorithm</h1>

<h2> Project Description</h2>
Access to restricted content is managed using an IP address allow list. These IP addresses are listed in the "allow_list.txt" file. A separate remove list specifies which IP addresses should no longer have access 
to this content. An algorithm is developed to automate the updating of the "allow_list.txt" file and delete the IP addresses that should no longer have access. The algorithm will parse a series of IP addresses that can access restricted information and will remove the addresses that are no longer alloweed automatically.
<br />


<h2>Program steps </h2>

- <b>Open the file that contains the allow_list</b> 
- <b>Read the file contents</b>
- <b>Convert the String into a list</b> 
- <b>Iterate through the allow list</b>
- <b>Remove IP addresses that are on the remove list</b>
- <b>Update the file with the revised list of IP addresses</b> 


<h2>IDE </h2>

<b>Jupiter notebook </b> 

<h2>Program walk-through:</h2>

<p align="left">
For the first part of the algorithm, I opened the "allow_list.txt" file and I assigned this
file name as a string to the import_file variable: <br/> <br />
<img src="https://imgur.com/nXTcqzh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
In the algorithm, the "with" statement is used with the .open() function in read mode to open
the allow list file for the purpose of reading it. The purpose of opening the file is to allow me to
access the IP addresses stored in the allow list file. The "with" keyword will help manage the
resources by closing the file after exiting the with statement. In the code with
open(import_file, "r") as file:, the open() function has two parameters. The first
identifies the file to import, and then the second indicates what I want to do with the file. In this
case, "r" indicates that I want to read it. The code also uses the as keyword to assign a
variable named file; file stores the output of the .open() function while I work within the
with statement:  <br/> <br />
<img src="https://imgur.com/FJtRKor.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
In summary, this code reads the contents of the "allow_list.txt" file into a string format
that allows me to later use the string to organize and extract data in my Python program. When using an .open() function that includes the argument "r" for “read,” I can call the .read() function in the body of the with statement. The .read() method converts the file into a string and allows me to read it.: <br/>
<img src="https://imgur.com/tNBUk2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
In order to remove individual IP addresses from the allow list, I needed it to be in list format.
Therefore, I next used the .split() method to convert the ip_addresses string into a list:  <br/> <br />
<img src="https://imgur.com/kEx9doc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
A key part of my algorithm involves iterating through the IP addresses that are elements in the
allow_list. To do this, I incorporated a for loop. Moreover, the algorithm requires removing any IP address from the allow list, ip_addresses, that is also
contained in remove_list. Because there were not any duplicates in ip_addresses, I was
able to use the following code to do this::  <br/> <br />
<img src="https://imgur.com/LLYtNV6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
As a final step in my algorithm, I needed to update the allow list file with the revised list of IP
addresses. To do so, I first needed to convert the list back into a string. I used the .join()
method for this. To rewrite the file, I appended the .write() function to the file
object file that I identified in the "with" statement:  <br/> <br />
<img src="https://imgur.com/U7ye5WP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The updated file is printed in this last section of the code:  <br/><br/>
<img src="https://imgur.com/Q3rE1JZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

