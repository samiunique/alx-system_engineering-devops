<a href="https://imgur.com/vK8tTwx"><img src="https://i.imgur.com/vK8tTwx.jpg" title="source: imgur.com" /></a>
<br>

Explanation or task 1:

Two Servers:
Introducing two servers for redundancy and to eliminate the Single Point of Failure (SPOF).

Load Balancer (HAProxy):
HAProxy is added to distribute incoming traffic across multiple web servers, improving performance and ensuring high availability.

Database Primary-Replica Cluster:
A Primary-Replica (Master-Slave) cluster is implemented for the database to enhance reliability and data redundancy.

Distribution Algorithm:
The load balancer is configured with a Round Robin distribution algorithm, which evenly distributes incoming requests among the web servers.

Active-Active vs. Active-Passive Setup:
The infrastructure is configured with an Active-Active setup. In this setup, all servers actively handle incoming requests, providing redundancy and load distribution. Active-Passive setup would involve standby servers that become active only if the primary server fails.

Database Cluster Operations:
The Primary node in the database cluster handles write operations, and the Replica nodes replicate data from the Primary and handle read operations. This improves both write and read performance.

Single Point of Failure (SPOF):
While the infrastructure addresses SPOF for web servers, the database cluster's Primary node could still be a potential single point of failure. Implementing failover mechanisms and redundancy for the Primary node can mitigate this.

Security Issues:
No firewall and lack of HTTPS introduce security vulnerabilities. Implementing a firewall, encrypting communication with HTTPS, and enforcing secure coding practices are essential for a secure infrastructure.

No Monitoring:
The infrastructure lacks monitoring, making it challenging to identify and address performance issues or potential failures. Implementing monitoring tools and practices is crucial for proactive maintenance.


