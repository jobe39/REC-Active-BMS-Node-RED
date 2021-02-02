# REC-BMS-Node-RED
Node RED flow for RS485 communication with REC Active BMS

This is a Node Red flow for communicating with REC Active BMS (http://www.rec-bms.com/ABMS.html).
It reads the most important figures and displays them in a dashboard. It also allows sending commands to the BMS for changes in Configuration (only one-value commands, which are the most of the existing commands).

For seeing the results of a command, you need to wait about 15 - 20 seconds. As the cycle is configured to read figures every 10 seconds. Only thing that needs to be changed is setting the correct com port in the serial node. 

Error handling is not really perfect :-). If wrong answers apply, the result is ignored and no resend is done (since it will be repeated after 10 seconds anyways). 

