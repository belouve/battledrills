
Aug 31

Your CIO hosts an open (passwordless) Zoom meeting in which an attacker joins and overhears the password to a public facing EC2 instance. The attacker gains access to the EC2 instance which holds PII of your clients.

What do you do? What’s next?

https://twitter.com/cybersecmeg/status/1432751792606023680?s=20

Contact Legal
Hopefully I paid for a firewall appliance so I can see how much if any of my data has been exfiltrated, while my team is reviewing how much data is out we are turning off the instance to preserve it's last run state. Time to assume the worst, call in a firm like mandient.
Remove the security groups to stop internet access, take a snapshot of the disk for the forensics nerds. Check if other instances use the same password. Involve legal as we determine what PII was exposed.

A lot of long days. Once data is compromised you can't un-compromise it.

Short version: get the attacker out as soon as possible, identify what was compromised, report the breach, review procedures to prevent a reoccurrence.

1. Snapshot the EC2 for forensics.
2. Follow the incident response policies of the company (which includes involving legal affairs).
3. Shutdown.
