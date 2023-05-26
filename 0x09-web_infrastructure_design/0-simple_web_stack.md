# EXPLAINED

A user wants to access a website hosted on a one server web infrastructure(this is becoming a hard word to spell or maybe it's just my brain) via www.foobar.com

### questions asked:

1. What is a server?

A server is a system that provides functionality for other programs or devices, called "clients". In this case, it stores and manages the web application, database and dependent files.

2. What is the role of the domain name?

The domain name is used to identify a website or online resource on the internet for easy recognition. For instance the domain name foobar.com is easier to remember than the IP address 8.8.8.8.

3. What type of DNS record www is in www.foobar.com?

In the DNS configuration for www.foobar.com, you would likely find a CNAME record that points "www" to the main domain or hostname of the Foobar website. This allows users to access the website by entering "www.foobar.com" in their web browser.

4. What is the role of the web server?

In this case, the web server (Nginx) hosts the website files and handles incoming requests from users accessing the website via www.foobar.com. It processes these requests, generating appropriate responses and delivers the website files users via web browsers.

5. What is the role of the application server?

An application server provides a platform for running computer programs. It is a type of middleware that sits between the database server and the end user.

6. What is the role of the database?

The database in this project is MySQL. It handles database-related operations such as storing users' information, retrieving dynamic contents and managing site functionality that requires data storage.

7. What is the server using to communicate with the computer of the user requesting the website?

The server uses the a set of rules known as Hypertext Transfer Protocol (HTTP) to communicate with the computer of the user requesting the website. Usually, when a user requests a web page, the browser sends an HTTP request to the server. The server then sends an HTTP response back to the browser, containing the requested web page.

### what the issues are with this infrastructure:

1. The issue with this infrastructure is that its reliance on a **single server**, implies that a failure in it will lead to the entire system. This failure will inhibit access to the website by users.

2. Downtime when maintenance needed (like deploying new code web server needs to be restarted):

When maintenance is needed in a system with a single point of failure (SPOF), the entire system will be unavailable until the maintenance is complete. This can lead to significant downtime, which can have a major impact on businesses.

3. Cannot scale if too much incoming traffic:

When there is too much incoming traffic, the SPOF will be overloaded and will eventually fail. This will cause the entire system to go down. The scaling options are limited in a SPOF infrastructure.
