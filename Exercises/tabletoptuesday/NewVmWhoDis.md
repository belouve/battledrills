
Sep 7

Your development team reports that they cannot access any of your org’s cloud instances. After further investigation, you find that MFA has been disabled for your clouds, and there are 50+ VMs spun up, that no one in your org created.

What’s next?

https://twitter.com/cybersecmeg/status/1435276265590857729?s=20

Crack a beer.
1. Conduct global password reset
2. Re-enable MFA
3. Preserve logs and review for unauthorized access 
4. Preserve vms (remove them from cloud but run analysis/collection) 
5. Review security posture
6. Check for data exfil, data access,etc
7. Review cyber insurance

If MFA is disabled, then your organization is owned. The attacker likely compromised the Admin account for your cloud IAM. You'd better engage a DFIR firm to conduct a comprehensive investigation and help you contain the incident.

ANALYSE - Does the cloud security console show anything? 
Can you work out what the VMs are doing - do they pose a direct and immediate threat to the org. Review logs to see what account removed MFA and created VMs. 
Is issue limited to just development team area?
Review alerts.

Oh and most importantly, stay calm - running around like a headless chicken helps no-one. Also, if you haven't positively identified this incident as being a false positive / innocent mistake / authorised activity, then give your IR team a heads up. Get them started.
