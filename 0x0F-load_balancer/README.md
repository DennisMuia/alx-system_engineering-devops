Project Title: Load Balancer Configuration
This project involves configuring a load balancer to distribute traffic to two web servers (web-01 and web-02) using the round-robin algorithm. The goal is to ensure that the web servers are identical, and to add a custom Nginx response header that tracks which web server is answering HTTP requests.

Task 0: Configure Nginx with a Custom HTTP Header
In this task, we need to configure Nginx to add a custom HTTP header (X-Served-By) to its HTTP response. The header's value should be the hostname of the server Nginx is running on.

To achieve this, we will use a Bash script (0-custom_http_response_header) to configure a brand new Ubuntu machine to match the task requirements. We will also ignore SC2154 for shellcheck.

Task 1: Install and Configure HAproxy
In this task, we need to install and configure HAproxy on our lb-01 server. The aim is to distribute traffic to web-01 and web-02 using the round-robin algorithm.

To achieve this, we will configure HAproxy to send traffic to the two web servers, making sure that HAproxy can be managed via an init script. We will also ensure that the servers are configured with the correct hostnames ([STUDENT_ID]-web-01 and [STUDENT_ID]-web-02).

To complete this task, we will write a Bash script (1-install_load_balancer) that configures a new Ubuntu machine to meet the above requirements.

Task 2: Add a Custom HTTP Header with Puppet
In this advanced task, we will automate the creation of a custom HTTP header response using Puppet. The header's name should be X-Served-By, and its value should be the hostname of the server Nginx is running on.

To complete this task, we will write a Puppet manifest (2-puppet_custom_http_response_header.pp) that configures a brand new Ubuntu machine to meet the above requirements.

Repository
All the files for this project can be found in the 0x0F-load_balancer directory of the alx-system_engineering-devops GitHub repository.
