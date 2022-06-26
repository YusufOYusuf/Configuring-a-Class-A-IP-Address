<h1>Configuring a Class A IP Address</h1>



<h2>Description</h2>
In this lab, I learned to configure a Class A IP address. In a Class A network, the first eight bits, or the first dotted decimal, is the network part of the address, with the remaining part of the address being the host part of the address. There are 128 possible
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 


<h2>Languages and Utilities</h2>

- <b>Windows Powershell<b>

<h2>Program walk-through:</h2>

<p align="center">
Right click the start Menu and open Network Connections: <br/>
<img src="https://i.postimg.cc/bvsn0jpk/Screen-Shot-2022-06-23-at-3-15-34-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
<br>
In the Network Connections window, double click the Ethernet network adapter:<br>
<img src="https://i.postimg.cc/Yq93X7C7/Screen-Shot-2022-06-25-at-7-00-07-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet status dialog box, click Properties:</br>
<img src="https://i.postimg.cc/HW4YSGP6/Screen-Shot-2022-06-25-at-7-03-48-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet Properties dialog box, under This connection uses the following items double click Internet Protocol Version 4(TCP/IPv4:  <br/>
<img src="https://i.postimg.cc/VvBX67gz/Screen-Shot-2022-06-25-at-7-05-28-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />


<br />
IN the Internet Protocol Cersion 4 (TCP/IPv4) Properties dialog box, select Use the following IP address and type in IP address,subnet mask,default gateway,preferred DNS server and alternate DNS Server:  <br/>
<img src="https://i.postimg.cc/SKS1pv67/Screen-Shot-2022-06-25-at-7-07-52-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />



<br />
Click start menu and open Windows powershell:  <br/>
<img src="https://i.postimg.cc/x1J5YZ4f/Screen-Shot-2022-06-23-at-3-31-44-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />




<br />
In Windows Powershell window execute the following command to get the IP address of the Ethernet network adapter: (Get-NetAdapter -Name "Ethernet 3" | Get-NetIPAddress).IPAddress:  <br/>
<img src="https://i.postimg.cc/76DKNQ6T/Screen-Shot-2022-06-25-at-7-12-26-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />





<br />
You will observe the IP address 1.2.3.4:  <br/>
<img src="https://i.postimg.cc/Kj1pK3j9/Screen-Shot-2022-06-25-at-7-13-54-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />







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
