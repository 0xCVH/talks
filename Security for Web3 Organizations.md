# Security for Web3 Organizations

> **TL;DR**: Make someone responsible for security, understand and secure your users & technology, use standard processes and review everything frequently

This is a simple guide for small and medium sized organisations with limited IT and cybersecurity expertise looking to setup a initial security strategy

This guide assumes you are:
- Fully or mostly remote team
- Have anonymous team members and/or contribuitors
- Using GitHub/GitLab for Software Development


## Security Responsible

- Make it someone's job (full or part time) to look after security for the organisation, or hire a third party consultant/advisor to help with this

## Mantain Lists

### Users
- **Detailed Records**: Maintain records for all team members and contributors, including names/usernames, contact details, roles, and access levels
- 
### Assets
- **End-User Devices**: Include all portable and mobile devices, recording hardware addresses, machine names, and owner details.
- **Network Devices & IoT**: Document networking and non-computing devices, with specific roles within the infrastructure noted.
- **Servers**: Catalog of server hardware, including each machine's function, operating system, and security configurations

### Software
- **Licensed and Cloud Services**: List of all software and cloud services used (e.g., Google, AWS, Slack), with details on who the admins are and contact points for support or in case of emergencies

## Secure Hardening and Configuration

### Users
- Enforce MFA and secure settings for all accounts, including personal and professional platforms as Twitter, Gmail, Discord, Telegram. Enforce the use of password vaults and hardware crypto wallets

### Assets
- Ensure all devices have anti-malware, firewalls, disk encryption, login authentication, auto lock-out mechanisms, and OS hardening. Implement secure DNS solutions, disable unnecessary ports/services like SSH, adopt Zero Trust Network architecture, utilize VPNs, enforce unique and complex passwords, enable automatic patching, and maintain detailed logs

### Software
- Implement SSO and MFA across all platforms, use hardware security keys for critical services, deactivate default accounts, enforce unique and complex passwords, set up automatic patching, and maintain comprehensive logs

### Domains & Email
- Secure configurations, DDOS Protection (e.g., Cloudflare), setup MFA, SPF/DKIM/DMARC, monitor DNS changes

### Software Development
- Enforce MFA, Secrets Scanning (e.g., GitHub, TruffleHog, GitGuardian), Branch Protection (PR Approvals, Signed Commits, no forced push), Static Code Analysis (e.g., CodeQL, Sonarcloud), Dependency Updates (e.g., Dependabots, Snyk), CI/CD Pipeline (e.g., GitHub Actions), Separate Environments (e.g., dev, staging, prod)

## Standard Operating Procedures (SOPs)

- **User On-boarding/Off-boarding**: Standardize onboarding tasks and preform background checks and recommendations. Ensure prompt deactivation of all accounts and access upon departure or extended leave
- **Patches, Upgrades and Deployments**: Define and enforce processes and checklists for each activity to avoid mistakes. Rollback plans are just as important!
- **Incident Response Process**: Establish clear protocols with contact points (e.g., https://securityalliance.org/), immediate actions, and post-mortem analysis procedures

## Recurrent Activities

- **Monthly/Quarterly Reviews**: Update all lists regularly, review access controls, ensuring appropriateness and necessity
- **Security Assessments**: Weekly vulnerability scans and annual or situational penetration testing and security audits of your products (e.g. after a major upgrade or a security incident)
- **Backups**: Secure and regularly update backups for all assets and software.
- **Monitoring**: Review security alerts regularly and take prompt action
- **Security Awareness**: Conduct security awareness and phishing campaigns for all team members

## Want to go further?

- https://www.cisecurity.org/controls/v8
- https://owasp.org/www-project-top-ten/
- https://www.nist.gov/quick-start-guides
