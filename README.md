<h1>Create New Folders in Bulk with PowerShell</h1>

<h2>Description</h2>
In this project, we’re going to use PowerShell to create new folders on our system in bulk.  I used this process to automate this manual administrative step for myself and my team at work. This project could be enhanced even more depending on your goal.
For this example, I’ll show you how to create new 12 folders for each month of the year.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Windows PowerShell ISE</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Walk-through:</h2>

<p align="center">
Launch the utility: <br/><br>
<img src="https://i.imgur.com/uEZGYaF.png" height="80%" width="80%" alt="PowerShell Steps"/>
<br />
<br />
Next, change directory. The PowerShell window may open with you in the USER folder by default. <br>You’ll need to change cirectory (cd) to the file location you want the folders to go:<br/><br>
<img src="https://i.imgur.com/kUxCUXi.png" height="80%" width="80%" alt="PowerShell Steps"/>
<br />
<br />
Begin creating your folder names inside quotations, and separated by a comma. If it’s easier for you to create all of the names in advance in a word processing app and format them with quotations and commas, I recommend you do so.
<br>
<br>After you've set up your folder names, you’ll need to tell PowerShell what you want to do with these by piping (|) to a command as follows: 
<br>
| %{New-Item -Name "$_" -ItemType "Directory"}  
<br/>
<br><img src="https://i.imgur.com/gyC8TO1.png" height="80%" width="80%" alt="PowerShell Steps"/>
<br />
<br />
<img src="https://i.imgur.com/9gAF2t8.png" height="80%" width="80%" alt="PowerShell Steps"/>
<br />
<br />
The end results. As we can see, the script successfully created these new folders to the specific location with one command.😊 <br/>
<br><img src="https://i.imgur.com/R9fGZku.png" height="80%" width="80%" alt="PowerShell Steps"/>
</br>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
