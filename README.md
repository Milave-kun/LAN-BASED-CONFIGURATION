# LAN-BASED-CONFIGURATION
## What is LAN BASED?
"LAN-based" typically refers to systems, devices, or
services that operate within a Local Area Network (LAN).
A LAN is a network that connects computers and devices
within a limited geographic area, such as a home, office, or
school. Devices in a LAN can communicate with each other
directly and share resources like files, printers, or internet
connections.

## LAN Based Examples
- LAN-based games: Multiplayer video games that allow players to connect and play with each
other over a local network instead of the internet.
- LAN-based file sharing: Systems where files are shared between computers connected to the
same LAN without needing to access external servers.
- LAN-based printing: Printers that are connected to a local network, allowing multiple users within
the network to send print jobs to them.
- LAN-based security systems: Surveillance or security systems that operate over a local network,
with cameras, sensors, and alarms connected to a central server within the same LAN.
- LAN-based systems: Software or systems that shares and passing data together to achieve
specific goal.

## Server
The server in this setup is typically the central system that
provides shared resources, such as a database, to the
clients.
## Client
A client is any computer or device that connects to the
server to request data or use services.

## Server Responsibilities
- Database Hosting: The server stores and manages the database, containing all
the data that clients need to access.
- Data Management: It handles all requests from clients, processing them and
sending back the appropriate data. For example, if a client needs to retrieve some
information, the server queries the database and returns the results.
- Centralized Control: It can control who has access to the database, typically
through user authentication and permissions.
- Data Integrity: The server ensures that the data remains consistent and
up-to-date across all clients.
- Requesting Data: Clients send requests to the server to retrieve or update data
stored in the database. For instance, a client might ask the server for customer
information, which is then returned for display or use.
- Interface: The client typically runs applications that interact with the server’s
database, like a web browser, database management tool, or a custom business
app.
- Local Processing: While the client may send requests to the server, it might also
perform local tasks, like displaying the data or making calculations.
- User Interaction: The client is where the user interacts with the data, through a
user interface (UI), and sends requests to the server.

# Server VS Clients
![image](https://github.com/user-attachments/assets/c327542e-6c09-4e1e-8eb0-4e72984c7496)

# APPLICATION
## Connect Computer 
Connect two Laptop/PC together.
<br>
It will give you network connection and assign you a dynamic ip address connection.
<br>
<br>
![image](https://github.com/user-attachments/assets/c7e173a0-a9c4-4841-9e1e-949b00352f47)

## Set Static IP Address for Server
Go to Network Connection, Properties and set static Ip Address.
<br>
In this config i will set the configuration
<br>
<br>
![image](https://github.com/user-attachments/assets/dc345e66-67ef-4ad1-8054-8da91dd8035b)

## Network Settings
Turn on Network Discovery
<br>
Turn on File and printer sharing
<br>
And also apply this to ALL Networks tab
<br>
<br>
![image](https://github.com/user-attachments/assets/58edff05-1b6e-4176-9b06-acc79d5bc2df)

## Set Static IP Address for Client
Set client static IP Address
<br>
We set the static ip address, because we wanted the ip address to be as is, or unchangeable even we disconnect our laptop.
<br>
<br>
![image](https://github.com/user-attachments/assets/99d86e03-f9b9-4b18-95cb-5893a431f54e)

## Check your IP Address : SERVER
Double check on cmd
<br>
Type ipconfig and you will see your static Ipv4 Address
<br>
<br>
![image](https://github.com/user-attachments/assets/cea31ff5-7b42-46ef-a8ef-1fc6ea4be7d0)

## Test Connectivity of Client : SERVER
Try PINGING the client
<br>
It will test, if your computer as server can find the IPAddress location of the client using cmd.
<br>
Type ping CLIENT IP
<br>
<br>
![image](https://github.com/user-attachments/assets/ce2515b5-3ef7-4ba1-adf0-54533d3359bc)

## Open SQL Server Config Manager : CLIENT & SERVER
Open SQL Server
<br>
Configuration Manager
<br>
<br>
![image](https://github.com/user-attachments/assets/7b7f14e0-e78e-4ebe-96f2-6e377da3a0fb)

## Enable TCP/IP : CLIENT & SERVER
Under Protocols for SQL EXPRESS
<br>
Enable TCP/P
<br>
<br>
![image](https://github.com/user-attachments/assets/4751e552-e74f-4717-906b-397d94ad25e3)

## Set IP Addresses : CLIENT & SERVER
Go to IP Addresses Tab
<br>
And set the TCP Port to 1433
<br>
This port is essential so don’t change it.
<br>
<br>
![image](https://github.com/user-attachments/assets/43e91ffb-fa92-40cd-b170-5bb5535e7bdd)
![image](https://github.com/user-attachments/assets/a6d425d7-3c4f-43ce-9d03-f6380ba4d2ca)

## SQL Server Browser : CLIENT & SERVER
As we can see SQL Server Browser was Stopped so we need to make it run.
<br>
Because it is essential for accessing SSMS between two computers.
<br>
<br>
![image](https://github.com/user-attachments/assets/fb5689ba-bae6-4c87-a112-073042edff36)

## Enable SQL Server Browser : CLIENT & SERVER
Go to Services
<br>
![image](https://github.com/user-attachments/assets/b17bf224-ffcd-4c22-8d0b-5f0b261ed4ca)
<br>
Go to it’s Properties and set Startup type to Automatic
<br>
Click Apply
<br>
Click Start to Run
<br>
<br>
![image](https://github.com/user-attachments/assets/f3885677-85de-4e0b-82aa-c180ec69aac0)

## Running SQL Server Browser : CLIENT & SERVER
As we can see SQL Server Browser Service was running.
<br>
<br>
![image](https://github.com/user-attachments/assets/8aa8a9bc-c478-44cf-872d-217a6ce37be8)

## Enable SQL Server Browser : CLIENT & SERVER
Right click SQL Server Browser Service and go to properties.
<br>
Set the Build-in account to Network Service
<br>
Click Apply
<br>
<br>
![image](https://github.com/user-attachments/assets/80a2c1b1-2ac2-412c-8e79-5fa58f75efd3)

## SQL Server : CLIENT & SERVER
Check the properties of SQL Server, set the Built-in account to Network Service.
<br>
<br>
![image](https://github.com/user-attachments/assets/53e63392-9fc0-4890-bbc8-e7e603d8b7d9)

## Restart SQL : CLIENT & SERVER
Go to your SQL Server Services and restart it.
<br>
It will apply all of our configuration to SQL
<br>
<br>
![image](https://github.com/user-attachments/assets/0b08176b-5ffd-4c3c-977a-f8f582d6e3a6)

## Open Windows Defender : CLIENT & SERVER
Open Windows Defender Firewall on both of the computer

## Inbound : CLIENT & SERVER
Under Inbound Rules, create new rule
<br>
SELECT PORT
<br>
<br>
![image](https://github.com/user-attachments/assets/e01759bc-3771-4cfd-a97e-309c0ea2c4f4)

## Set TCP PORT : CLIENT & SERVER
Select TCP
<br>
And set the Specific local ports to 1433
<br>
<br>
![image](https://github.com/user-attachments/assets/d5f9513d-d8ba-44b8-b244-ffe516ba3f50)

## Allow Connection : CLIENT & SERVER
Then allow the connection for this inbound network
<br>
<br>
![image](https://github.com/user-attachments/assets/da356219-d261-42bf-ba96-23d2c058e64a)

## Add Publicity : CLIENT & SERVER
Check all and click next
<br>
<br>
![image](https://github.com/user-attachments/assets/93e21d95-8d19-40b3-a4f2-8b3a5cc3e5cc)

## Inbound Name : CLIENT & SERVER
Name your Inbound and click Finish to save
<br>
<br>
![image](https://github.com/user-attachments/assets/f37603ab-de9b-41ad-9da6-eacdb42ca2e1)

## Inbound : CLIENT & SERVER
Now you can see your Inbound connection to the list
<br>
<br>
![image](https://github.com/user-attachments/assets/05357121-0fe2-4b10-b1ea-91be14f9c2da)

## Outbound : CLIENT & SERVER
Under Outbound Rules just repeat the steps
<br>
Create new rule
<br>
Set the port and tcp
<br>
Allow the connection
<br>
Set publicity
<br>
Name it And save
<br>
<br>
![image](https://github.com/user-attachments/assets/e65e632d-8a10-46e6-b766-bc5cf9aae435)

## SSMS Login : SERVER
IMPORANT
<br>
[
<br>
CREATE FIRST NEW DATABASE, name it activity
<br>
]
<br>
Open your SSMS login as Windows Login and create new Login under Security.
<br>
<br>
![image](https://github.com/user-attachments/assets/1cac6ec8-7b7f-4d19-9679-2da5895c5708)

## Login Credentials : SERVER
Name your Login, Set the passwords
<br>
<br>
![image](https://github.com/user-attachments/assets/15854674-8e3c-411f-a507-ce9298e26878)

## Set User Mapping : SERVER
Go to your Login credential, and right click, go to properties.
<br>
Under User Mapping select your database to access. 
<br>
<br>
![image](https://github.com/user-attachments/assets/51f4a8ec-ccf6-4fb9-883b-0389ca1670ae)

## Login List : SERVER
Now after saving you can see your login credential saved in the List
<br>
<br>
![image](https://github.com/user-attachments/assets/59aa1632-d763-4904-ba21-083c3ca9f4ad)

## Server Properties : SERVER
Right click and go to properties
<br>
<br>
![image](https://github.com/user-attachments/assets/6e4cbbeb-4ddc-4647-bbbf-9431f1913143)

## Allow SQL Server Auth : SERVER
Allow SQL Server and Windows Authentication mode
<br>
<br>
![image](https://github.com/user-attachments/assets/10189d98-2d29-4203-a52a-0da689b13993)

## Try Loging in : SERVER
Connect again on your SSMS,
<br>
Select Authentication as SQL Server Authentication then Login via your created login credentials.
<br>
<br>
![image](https://github.com/user-attachments/assets/d2d91577-d288-4bce-984d-7befdaf45773)

## Login List : SERVER
If you logon, you can see another database was created.
<br>
But it was login via SQL Server Authentication
<br>
<br>
![image](https://github.com/user-attachments/assets/92fd765c-6f51-4dd0-8896-ebbafbe6596e)

## Create Project : CLIENT
Go to Visual Basic create Server Project Create VB Project for client, name it as ClientPC
<br>
<br>
![image](https://github.com/user-attachments/assets/1a7ae868-3424-45ca-a542-344c4d26b987)

## Client Connection : Client
Go to Server Explorer and add new SQL Connection.
<br>
Set the Server name as the same Ip Address we created before.
<br>
Use SQL Server Authentication, put your login, and select your database.
<br>
<br>
![image](https://github.com/user-attachments/assets/8416c460-e5ad-4d91-9dca-347e5b0f285d)
<br>
As we can see, we successfully access the Server from the CLIENT. And make server SQL Connection in VB.
<br>
Now we can create normalprojects in VB using this SQL Connection.

## Application : Client
Just reapply our last topic about MODULE and we can create new project out of it.
<br>
<a href="https://github.com/Milave-kun/Registration-Form-ASP.NET">
Registration Form
</a>




















