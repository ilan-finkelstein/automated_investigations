This is the initial code for an automated investigation process to  determine if an IP address is related to a cloud provider or Barracuda and to send the determination to a slack channel. 
This code is meant to sit behind an api gateway and recieve a Post from CudaLogs with the alert in the IP field of the headers if an alert is triggered. The goal is to eliminate the need to kick off the initial alert and automate initial investigation tasks.
The postman version is intended to be used without an api gateway, great for testing without generating an event in CudaLogs.
These are to be considered v1 and will updated to perform judgements and then communicate with a second lambda that will handle slack comms.
