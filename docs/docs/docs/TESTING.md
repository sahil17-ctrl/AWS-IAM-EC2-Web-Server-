Testing Plan — AWS IAM & EC2 Web Server

1. Repository Checks

- [ ] Confirm "index.html" exists in the repository.
- [ ] Confirm the README and deployment documentation are available.

2. EC2 Deployment Checks

- [ ] Confirm the EC2 instance is running.
- [ ] Confirm Apache is installed and running.
- [ ] Confirm "index.html" is placed in the web server's document root.
- [ ] Open the website using the EC2 public address.

3. Network Checks

- [ ] Confirm HTTP traffic on TCP port 80 is allowed by the Security Group.
- [ ] Confirm SSH access is restricted to a trusted IP address.
- [ ] Confirm unnecessary inbound ports are not exposed.

4. IAM Checks

- [ ] Review the IAM user's assigned permissions.
- [ ] Confirm permissions follow the principle of least privilege.
- [ ] Verify access is limited to the resources required for the task.

5. Evidence

Record the actual test date, results, and screenshots after performing each test.

Important: Do not mark a test as passed until it has been performed and verified.

Current Status

The project files are uploaded to GitHub. AWS deployment tests remain pending until the EC2 website is deployed.
