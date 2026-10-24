AWS IAM & EC2 Web Server Architecture

Overview

This project demonstrates how a static website can be hosted on a Linux Amazon EC2 instance using Apache HTTP Server.

Architecture Flow

Visitor's Browser
|
v
Internet
|
v
EC2 Security Group
(HTTP - TCP Port 80)
|
v
Linux EC2 Instance
|
v
Apache HTTP Server
|
v
index.html

AWS Components

- Amazon EC2: Runs the Linux web server.
- Security Group: Controls inbound and outbound network traffic.
- IAM: Manages identities and permissions for AWS access.
- Apache HTTP Server: Serves the static website to visitors.

Security Considerations

- Allow only the network ports required for the project.
- Restrict SSH access to a trusted IP address.
- Apply least-privilege IAM permissions.
- Never store AWS credentials or private keys in the repository.

Deployment Status

The source code is available in this repository. The live EC2 deployment must be completed and verified separately.
