May 18

Your AV/EDR alerts you that 10 systems (that are hybrid domain-joined) have malware on them. After further investigation, you determine they are being used for crypto mining. 

What more info do you collect, and what do you do next?

https://twitter.com/cybersecmeg/status/1394845551351447555?s=20

----

Step 1 is isolate, THEN notify. The issue is that we don’t know what else might be included in the payload, and we have to assume that data could be exposed to leakage or ransomware.

what data did you collect to make this decision, and are you going to alert anyone (like the users and their managers) before isolating the systems? if one of the users is the CEO, are you going to alert them or their executive assistant?

Packet capture of those machines to see what they are talking to and try to find a sample of the miner software to examine to determine extent of damage.

(Are we isolating?)
Only after threat analysis has been performed and it has been determined that in doing so will mitigate the threat (to some extent). From there determine how to clear the threat and setup event alerts to catch the threat earlier or determine further threat scope
I’m sure during this point in time we would involve the appropriate authorities. At the very least report it up. Since we have already done our homework and have some baseline data, it could be used as evidence. Also we would share any threat intel we collected.

Interesting note:  ’m not sure 10 compromised machines being used for crypto mining is worthy of being reported to the feds (it’s generally not unless you’re incurring a large loss). but absolutely you would follow your incident response procedures and report it up the chain of command! Smiling face with smiling eyes

----
identify purpose of the system(s) 

identify level of risk to org.

draft comms

identify user that executed process, 

identify all user and service accounts that are domain joined that have logged into that machine in the last 90

review tertiary logs, hypervisor, switch, etc.

identify business impact of resetting accounts and isolating the systems. 

once approved, coordinate efforts between responsible teams to reset accounts and cut off network access. in parallel, block external IP's at the boundary and w/ all EDR agents. 

once isolated..

engaged DF, look into memory, disk, logs, etc. 

identify actions taken by compromised user account (move this step up a few) 

determine full scope of access. 

begin overall timeline.

send updated comms with findings, chat with legal, get a beer and call it a day.

----
