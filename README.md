# V Profile Project - Local Setup
Hey there! I just wrapped up my V Profile Project, where I successfully set up a multi-tier web application stack on my local machine. This project was a fantastic way to dive into the world of DevOps and prepare for even bigger challenges ahead.

# What I Did
# Set Up a Multi-Tier Web App Stack
I started by setting up a complete web application stack that powers a social networking site written in Java. Here’s a breakdown of what I worked with:

- Nginx: I configured Nginx as a load balancer to efficiently manage incoming traffic and distribute it to the right services.
- Apache Tomcat: I deployed the Java web application on Tomcat, which handles the server-side logic.
- RabbitMQ: Even though RabbitMQ was included as a dummy service for complexity, it was a great opportunity to get familiar with message brokers.
- Memcached: I implemented Memcached for database caching, significantly speeding up data retrieval and reducing load on MySQL.
- MySQL: MySQL was set up as the database, where all user information and other crucial data are stored.

# Automated the Entire Setup with Vagrant
To streamline the process, I used Vagrant to automate the setup of virtual machines for each service. This made the setup repeatable and efficient, saving me from manually configuring each VM.

# Tested and Validated the Stack
After everything was up and running, I thoroughly tested the stack to ensure all the services were communicating as expected:

- Verified that Nginx properly routed traffic to the Tomcat server.
- Confirmed that user data was being stored and retrieved correctly from MySQL.
- Checked that Memcached was effectively caching database queries.
- Ensured RabbitMQ was integrated into the setup, even though it was non-functional for now.

# Laid the Groundwork for Future Projects
This project was more than just a one-off setup—it laid a solid foundation for future projects. Here’s what’s coming next:

# Deployment on Different Platforms: 
- I’ll be deploying similar setups in different environments.
# Refactoring and Containerization: 
- The next step will involve refactoring the app and containerizing it for better scalability and manageability.
# Kubernetes Deployment: 
- Eventually, everything will be managed within a Kubernetes cluster, and this project provided the baseline knowledge I’ll need.

# Why This Was Important
Completing this project served two key purposes:

# Establishing a Baseline: 
- This setup was crucial for understanding how different services work together in a multi-tier architecture. It’s the starting point for more complex projects down the line.

# Building a Local R&D Lab: 
- Now that I have this stack set up locally, I have a personal lab where I can experiment freely. Whether it’s testing new configurations or practicing troubleshooting, I have a safe environment to learn in.
# Prerequisites
#
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later

# Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
# Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

Then look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql


