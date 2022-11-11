#### Background:
A typical FTP session operates using two channels:
	1) Command or Control channel - transmits commands
	2) Data channel - tranfers data

**Active vs Passive**
The FTP server may support either Active or Passive connections, or both. 

-   In an Active FTP connection, the client opens a port and listens. The server is required to actively connect to it. 
-   In a Passive FTP connection, the server opens a port and listens (passively) and the client connects to it. 

This separation of command information and data into separate channels is a way of being able to send commands to the server without having to wait for the current data transfer to finish. If both channels were interlinked, you could only enter commands in between data transfers, which wouldn't be efficient for either large file transfers, or slow internet connections


#### Enumerate:

**Nmap:**
``


