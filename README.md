<h1>File Update Through A Python Algorithm</h1>

<h2> Project Description</h2>
Access to restricted content is managed using an IP address allow list. These IP addresses are listed in the "allow_list.txt" file. A separate remove list specifies which IP addresses should no longer have access 
to this content. An algorithm is developed to automate the updating of the "allow_list.txt" file and delete the IP addresses that should no longer have access. The algorithm will parse a series of IP addresses that can access restricted information and will remove the addresses that are no longer alloweed automatically.
<br />


<h2>Program steps </h2>

- <b>Open the file that contains the allow_lsit</b> 
- <b>Read the file contents</b>
- <b>Convert the String into a list</b> 
- <b>Iterate through the remove list</b>
- <b>Remove IP addresses that are on the remove list</b>
- <b>Update teh file with the revised list of IP addresses</b> 


<h2>IDE </h2>

<b>Jupiter notebook </b> 

<h2>Program steps:</h2>

<p>
  
- <b> The code begins with the appropriate
import lines to include the essential libraries for data processing and file handling, such as
pandas and json</b> 
  
- <b> Import modules such as os.path, time, and random for further functionality</b>

- <b> A dictionary named "available_products"; is constructed to contain
the initial fruit data. Each fruit is represented by a unique product ID, and its data such as name,
price, origin, quantity, and date are saved as dictionary values</b>

- <b> The json.dumps() function is used
to convert the dictionary to JSON format, and the resultant JSON string is saved to a file named
"data.json" for database storage</b>

- <b> The code then specifies two primary functions: &quot;admin()&quot; and
"user()". The "admin()" function handles administrative activities, whereas the "user()" function
handles user-specific functions.</b>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
