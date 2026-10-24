Security Guidelines

IAM Best Practices

- Follow the principle of least privilege.
- Avoid using the AWS root account for everyday tasks.
- Grant only the permissions required for the task.
- Review IAM permissions regularly.

EC2 Security

- Allow SSH (TCP port 22) only from your trusted IP address.
- Allow HTTP (TCP port 80) for public website access.
- Do not expose unnecessary ports.
- Keep the operating system and web server updated.

Credential Protection

- Never upload AWS access keys, passwords, or private ".pem" keys to GitHub.
- Do not hardcode credentials in website files.
- Protect SSH private keys and store them securely.

Cost Awareness

- Check AWS pricing before launching resources.
- Stop or terminate resources when no longer needed.
- Remember that some resources, such as EBS volumes, may continue to incur charges.
