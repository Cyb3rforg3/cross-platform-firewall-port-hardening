## Firewals Rules Setup

## step by step process to allow/block ports

1. press Win + R, type wf.msf -> Enter
2. Go to Inbound Rules -> New Rule
3. Choose Port -> Click Next
4. Choose TCP or UDP
5. Enter specific port numbers (eg: 21,23,445)
6. select Block/Allow the connection
7. Apply to Domain, Private, Public
8. Give a meaningful name: Block Telnet 

> Repeat for Outbound Rules if you want full control

## Important Information
>> Safe ports to Block (For Most System)
1. 21 (FTP)
2. 23 (Telnet)
3. 135-139 (NetBIOS)
4. 445 (SMB)
5. 1433, 1434 (SQL Server)
6. 3389 (RDP) [if not used]
