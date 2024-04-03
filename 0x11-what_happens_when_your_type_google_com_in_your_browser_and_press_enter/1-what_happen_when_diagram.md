
https://medium.com/@yitesam/lets-shed-light-on-what-occurs-when-you-input-google-com-into-your-browser-and-hit-enter-778d8ea9c803

Let’s shed light on “what occurs when you input ‘google.com’ into your browser and hit enter”!
Samson Mekonnen
Samson Mekonnen

3 min read
·
22 hours ago





Let’s delve into the intricacies of servers, a term integral to our discussion.

Defining a Server:
A server is a software or hardware entity that furnishes services to another program or device, termed the client, in what is known as the client-server model.

Understanding the Client-Server Model:
In this model, the client, often a web user’s internet-connected device such as a computer, laptop, or smartphone, communicates with the server to request information. The client typically employs web-accessing software like Google Chrome, Firefox, or Safari. In our scenario, the client is represented by the browser we use to input “www.google.com."

The Role of Servers:
Conversely, the server is responsible for providing or serving information to the client. Servers store webpages, sites, or applications. In our case, the Google server fulfills this role.

Initiating Access:
When a client device seeks to access a webpage, it sends a request to the server, which then downloads a copy of the webpage onto the client’s device for display in the user’s web browser.

Navigating the Internet’s Phonebook:
Entering a website name or address, technically known as a URL (Uniform Resource Locator), like https://www.google.com into our browser and pressing Enter triggers a series of actions. Firstly, the browser dissects the URL into its components. To achieve this, it relies on Domain Name System (DNS) servers.

Demystifying URLs:
URLs consist of various parts, including the protocol, hostname, port, and path-and-file-name. For our discussion, we’ll focus on the protocol and hostname. In the example https://www.google.com, “https” signifies the protocol, and “www.google.com" denotes the hostname, which can be a domain or an IP address.

Decoding DNS:
The Domain Name System (DNS) functions as the internet’s equivalent of a phonebook. DNS servers translate human-readable domain names into machine-readable IP addresses, facilitating device identification and communication.

The DNS Resolution Journey:
DNS resolution, or DNS lookup, involves four key steps and servers:

1. DNS recursor: Receives queries from clients and either retrieves the IP address from its cache or initiates further requests.
2. Root server: Directs requests to the appropriate Top-Level Domain (TLD) server.
3. TLD server: Manages the last portion of a hostname, such as “.com,” and forwards requests to the authoritative nameserver.
4. Authoritative nameserver: Returns the IP address for the requested hostname or reports an error if the record is unavailable.

<a href="https://imgur.com/QxYexUN"><img src="https://i.imgur.com/QxYexUN.png?1" title="source: imgur.com" /></a>

Establishing Connection:
Once the browser identifies the location of www.google.com, it initiates a connection to access the website. This connection is established using internet protocols, notably the Internet Protocol Suite or TCP/IP, governing data transmission over networks.

Managing Traffic and Security:
Before data transfer begins, traffic control measures come into play. Load balancers distribute incoming traffic across multiple servers to prevent overloading. Additionally, firewalls safeguard against unauthorized access by filtering traffic based on predefined security rules.

Enhancing Security with SSL:
Secure Socket Layer (SSL) protocol ensures data privacy during transmission between servers and browsers. SSL certificates establish encrypted links, rendering intercepted data incomprehensible to unauthorized entities.

Identifying Secure Connections:
We can recognize SSL-secured websites by the presence of a padlock icon and “https://” in the URL.

Differentiating HTTP and HTTPS:
HTTP (HyperText Transfer Protocol) and its secure counterpart HTTPS facilitate communication between web browsers and servers. While HTTP is widely used, HTTPS incorporates SSL for enhanced security.
<br>
<a href="https://imgur.com/Z8penVf"><img src="https://i.imgur.com/Z8penVf.jpg" title="source: imgur.com" /></a>
<br>
Understanding HTTP Methods and Response Codes:
HTTP requests utilize various methods, such as GET, POST, PUT, and DELETE, to interact with web servers. Response codes indicate the success or failure of these requests, categorized into informational, successful, redirection, client error, and server error responses.

Navigating Web and Application Servers:
Web servers deliver static content like HTML pages, images, and text files, while application servers handle dynamic content, enabling user interaction and data manipulation.

Emphasizing the Database Role:
Database servers manage data storage and retrieval, interacting with databases to perform operations like adding, modifying, or retrieving data. Relational and non-relational databases are commonly used for this purpose.
<br>
<a href="https://imgur.com/7ynbRZy"><img src="https://i.imgur.com/7ynbRZy.jpg" title="source: imgur.com" /></a>
<br>
In Summary:
The process of accessing a website like www.google.com involves a series of intricate steps, from DNS resolution to data transmission and security measures. Although these processes occur swiftly, understanding them enhances our appreciation of the technology behind web browsing.
