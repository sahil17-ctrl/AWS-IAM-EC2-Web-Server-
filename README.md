# AWS IAM & EC2 Web Server

A beginner Cloud & DevOps internship project package for learning IAM fundamentals, launching a Linux EC2 instance, configuring a Security Group, and hosting a static website with Apache.

## Current status
Project source and documentation are prepared. **AWS deployment and the live website are not completed by this repository alone.** Follow the checklist and only report steps you actually complete.

## Learning objectives
- Understand IAM users, groups, roles, policies, permissions, and least privilege.
- Launch and connect to a Linux EC2 instance.
- Configure Security Group ingress safely.
- Install Apache and host `index.html`.
- Document the deployment and verify the website.

## Repository contents
- `index.html` — responsive static website
- `docs/DEPLOYMENT.md` — EC2 deployment checklist
- `docs/SECURITY.md` — IAM and network security notes
- `docs/ARCHITECTURE.md` — system architecture
- `docs/TESTING.md` — test plan and evidence checklist
- `docs/LINKEDIN_POST.md` — suggested post, to use only after actual deployment
- `docs/COVER_LETTER_TEMPLATE.md` — optional paper-submission cover letter template, unrelated to this AWS project

## Architecture
Visitor browser → Internet → EC2 Security Group (HTTP TCP/80) → Linux EC2 → Apache HTTP Server → `index.html`

IAM controls AWS identity and permissions. Security Groups control network traffic; these are separate security layers.

## Setup checklist
- [ ] Check AWS pricing and Free Tier eligibility before creating resources.
- [ ] Launch a Linux EC2 instance.
- [ ] Restrict SSH TCP/22 to your trusted IP or use a safer managed connection method.
- [ ] Allow HTTP TCP/80 for the public demo.
- [ ] Install and start Apache.
- [ ] Copy `index.html` to the web server document root.
- [ ] Test the page from a browser using the instance's public address.
- [ ] Add genuine screenshots and update the project status.
- [ ] Stop/terminate unused resources; EBS storage and other resources can still incur charges.

## Security
Never commit AWS access keys, passwords, `.pem` private keys, or other secrets. Avoid root credentials for everyday administration. Use least-privilege permissions.

## Live website
Add a working URL only after deploying and testing:
`Not deployed yet`

## Author
Update with your correct name, college, and date if needed.
