NCIDENT REPORT
INCIDENT SUMMARY
The incident constituted a server failure on our online shopping web application. It lasted a duration of one hour from 2.00 P.M to 3.00 P.M. It impacted our clients in the following ways: the clients could access their accounts, they couldn’t process their orders, they couldn’t check on the available goods and they couldn’t add items to their cart. The server failure was caused by a lot of user requests that it couldn’t handle the traffic. The server is built to support 100 customers concurrently but at that particular moment there were around 120 customers.

TIMELINE
Time of detection: 2.05P.M
How was the issue detected: A customer complaint on our hotline. She was already logged in but couldn’t add items to her cart.
Actions taken: The physical server and the web server software. The assumption was that either the physical server had failed or the web server software.
Debugging: The internet connection was probed but it was functional.  
Team escalated to: The issue was escalated to the technical department. The head engineer was working to resolve the issue as fast as possible.
Resolution: The operations were transferred to the back-up server. The system was up in running in around one hour. 

ROOT CAUSE	
The root cause was the web server software. The software couldn’t handle the number of customer requests. It is built up to handle one hundred requests concurrently and at that particular time it had requests margining on one hundred and twenty. The software doesn’t have the capabilities to handle all the requests and gives out. The physical server was also overworked and started overheating. It was a problem that led to another problem. A chain of problems that made the resolution time longer.
The issue was fixed by bringing up the backup server which is always on standby. it is not running so we had to give it time to boot hence the hour delay. Data logs are usually stored periodically on that server and the most recent transactions are available. 

CORRECTIVE AND PREVENTATIVE MEASURES
Setting another physical server that is always on stand-by. Having more than one server will greatly reduce the chances of failure by increasing redundancy. We also greatly benefit by adding a monitoring system to capture the issue before the customer realizes and at the fastest time possible. This will make it easier to tackle the problems with ease and at the point of failure.


