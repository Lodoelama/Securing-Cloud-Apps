# Securing Cloud Apps 

## Your Web Application

Enter the URL for the web application that you created:

[https://lodoesecurityblog.azurewebsites.net/](https://lodoesecurityblog.azurewebsites.net/)

### Screenshots

![cyberblog1](https://github.com/Lodoelama/Securing-Cloud-Apps/assets/125059539/517f4c7c-1a26-4c1e-8e19-49c8d7967a89)
![cyberblog2](https://github.com/Lodoelama/Securing-Cloud-Apps/assets/125059539/fb779eaa-d1da-420e-8fb6-c8ba4b0342da)
![cyberblog3](https://github.com/Lodoelama/Securing-Cloud-Apps/assets/125059539/358f35ad-9b03-4457-8907-dd13c42744ae)


## Day 1 Questions

### General Questions

1. What option did you select for your domain (Azure free domain, GoDaddy domain)?
   
   Azure free domain

2. What is your domain name?

   lodoesecurityblog.azurewebsites.net

### Networking Questions

1. What is the IP address of your webpage?

   20.37.196.200

2. What is the location (city, state, country) of your IP address?

   Sydney, New South Wales, Australia

3. Run a DNS lookup on your website. What does the NS record show?

   The DNS lookup for this domain did not return a traditional NS record. However, the response indicates ns1-06.azure-dns.com as the primary name server.

### Web Development Questions

1. When creating your web app, you selected a runtime stack. What was it? Does it work on the front end or the back end?

   I selected the PHP 8.2 runtime stack. It works on the back end as part of the server-side execution of PHP code.

2. Inside the `/var/www/html` directory, there was another directory called assets. Explain what was inside that directory.

   Inside the assets directory, there are two subdirectories: `css` and `images`. The `css` directory is responsible for the visual aspect of the webpage, while the `images` directory holds image files used in the web app.

## Day 2 Questions

### Cloud Questions

1. What is a cloud tenant?

   A cloud tenant is a logical grouping of resources and services within a cloud environment.

2. Why would an access policy be important on a key vault?

   An access policy on a Key Vault is important to provide granular control over access permissions, enhance security, meet compliance requirements, enable auditing, and facilitate collaboration and delegation of tasks related to cryptographic assets stored in the Key Vault.

3. Within the key vault, what are the differences between keys, secrets, and certificates?

   - Keys: Used for cryptographic operations such as encryption and signing.
   - Secrets: Store sensitive information like passwords or API keys.
   - Certificates: Used for secure communication and authentication.

### Cryptography Questions

1. What are the advantages of a self-signed certificate?

   - Cost-effective
   - Quick to deploy
   - Provides control over the certificate generation process
   - Enables encryption and secure communication

2. What are the disadvantages of a self-signed certificate?

   - Lack of trust by clients
   - Potential compatibility issues with certain applications or systems
   - Need for manual distribution of trust

3. What is a wildcard certificate?

   A wildcard certificate is an SSL/TLS certificate that secures a domain and all its subdomains with a single certificate. It uses a wildcard character (*) to match any subdomain.

4. When binding a certificate to your website, Azure only provides TLS versions 1.0, 1.1, and 1.2. Explain why SSL 3.0 isn't provided.

   SSL 3.0 is not provided due to security concerns and vulnerabilities associated with this protocol.


## Day 3 Questions

### Cloud Security Questions

1. What are the similarities and differences between Azure Web Application Gateway and Azure Front Door?

   - Azure Web Application Gateway: Advanced application delivery with URL routing and WAF features.
   - Azure Front Door: Global CDN with advanced traffic routing capabilities, primarily focused on performance optimization and global load balancing.

2. What is SSL offloading? What are its benefits?

   SSL offloading is the process of terminating SSL/TLS encryption at the load balancer or edge server. Its benefits include reduced server load, simplified certificate management, centralized security enforcement, flexibility in backend server technologies, and performance optimizations.

3. What OSI layer does a WAF work on?

   A WAF (Web Application Firewall) works on the Application Layer (Layer 7) of the OSI model.

4. Select one of the WAF managed rules (e.g., directory traversal, SQL injection, etc.), and define it.

   - Rule: SQL Injection
   - Definition: Designed to protect web applications from SQL injection attacks. It analyzes incoming requests and detects suspicious SQL code patterns in input parameters to prevent unauthorized access, data breaches, and data manipulation.

### Hypothetical Scenario

Consider the rule that you selected. Could your website (as it is currently designed) be impacted by this vulnerability if Front Door wasn't enabled? Why or why not?

Since my website doesn't have any input fields and database interactions, the possibility of it being impacted by the SQL injection vulnerability is low, even if Azure Front Door is not enabled.

### Day 3 Activities

![azurefrontdoor](https://github.com/Lodoelama/Securing-Cloud-Apps/assets/125059539/82e54d4a-b37b-4652-a5b2-faa4bcc5ac6e)
![customrule](https://github.com/Lodoelama/Securing-Cloud-Apps/assets/125059539/e23676cc-12af-4a83-a277-b436c34261df)


## Disclaimer on Future Charges

Please type "YES" after one of the following options:

- Maintaining website after project conclusion: I am aware that I am responsible for any charges that I incur by maintaining my website. I have reviewed the guidance for minimizing costs and monitoring Azure charges.

- Disabling website after project conclusion: I am aware that I am responsible for deleting all of my project resources as soon as I have gathered all of my web application screenshots and completed this document.

YES

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
