# Base Image 
FROM ubuntu:16.04 

# Maintainer of this Image 
MAINTAINER Amit Vashist <turabvit@gmail.com>

# Initalize APT Repo. 
RUN apt-get update 


# Install Apache Packages 
RUN apt-get install apache2 -y 

# Inject Custom Web Page
COPY amit.html /var/www/html/hello.html


# Bring up the Apache App. 
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
