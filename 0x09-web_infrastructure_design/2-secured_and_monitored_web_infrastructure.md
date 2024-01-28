<a href="https://imgur.com/L8keAKW"><img src="https://i.imgur.com/L8keAKW.jpg" title="source: imgur.com" /></a>
<br>

explanation for task 2:

Firewalls:
Firewalls are added to control and monitor incoming and outgoing traffic, acting as a secure gateway. They help protect the infrastructure from unauthorized access and potential security threats.

SSL Certificate (HTTPS):
An SSL certificate is added to enable HTTPS, encrypting traffic between the user's browser and the web server. This enhances security by protecting data in transit, preventing eavesdropping and tampering.

Monitoring Clients:
Monitoring clients, such as Sumologic, are used to collect and analyze logs and metrics from various components in the infrastructure. This helps in identifying performance issues, security incidents, and ensuring system health.

Terminating SSL at Load Balancer:
Terminating SSL at the load balancer is an issue because it means that traffic between the load balancer and web servers is unencrypted. To address this, communication between the load balancer and web servers should also be encrypted (end-to-end encryption).

MySQL Server Write Capability:
Having only one MySQL server capable of accepting writes is a potential issue as it creates a single point of failure. Implementing a Primary-Replica cluster with multiple nodes can improve availability and distribute the write load.

Servers with Same Components:
Having servers with identical components (database, web server, application server) might be a problem because it lacks diversity and introduces a potential single point of failure. Introducing diversity in server types and distributing components can enhance resilience.

Terminating SSL at Load Balancer:
As mentioned, terminating SSL at the load balancer without re-encrypting traffic to the web servers leaves internal communication unencrypted, potentially exposing sensitive data.

Single MySQL Server for Writes:
Relying on a single MySQL server for write operations creates a bottleneck and a single point of failure. A Primary-Replica cluster is recommended for redundancy and improved write performance.

Identical Components on Servers:
Having servers with the same components introduces a risk of a widespread failure if a common issue affects all servers. Introducing diversity in server roles and components helps in building a more resilient infrastructure.