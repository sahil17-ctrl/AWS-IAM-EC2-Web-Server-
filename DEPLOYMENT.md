# EC2 + Apache Deployment Checklist

> Follow this in your own AWS account. Exact commands depend on the AMI you choose.

1. Review AWS pricing, Free Tier eligibility, and expected resource costs.
2. Launch a suitable Linux EC2 instance and securely store the key pair.
3. Configure the Security Group: allow inbound HTTP TCP/80 for the demo. Restrict SSH TCP/22 to your trusted IP; do not expose SSH to `0.0.0.0/0`.
4. Connect using the recommended method for your AMI.
5. Install Apache using the AMI's package manager (Amazon Linux commonly uses `dnf`/`yum`; Ubuntu commonly uses `apt`).
6. Start and enable the Apache service.
7. Copy `index.html` to the web server document root (commonly `/var/www/html/`, but confirm for your AMI).
8. Open `http://<EC2-PUBLIC-IP>/` in a browser and verify the website.
9. Take genuine screenshots of the instance status, safe Security Group configuration, and working website.
10. When finished, stop or terminate unneeded resources. EBS volumes, snapshots, Elastic IPs, and other resources can incur charges independently.

Do not mark deployment complete until the site has been tested.
