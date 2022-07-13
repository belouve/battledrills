A disgruntled senior security engineer abruptly quits your organization, and you notice that your team (SOC, IR, etc.) no longer has access to any of your security tools. The employee who quit had access to all of your org’s critical data.

What do you do?

https://twitter.com/cybersecmeg/status/1501250902925230084?s=20&t=Pg2WhD8l4LT42tcUfgnFlg


Recognize you done fucked up on multiple levels. Id suggest other things, but this was such a control AND personel failure that there isnt much in the scenario that would lead me to believe anything but the disgruntled employee having you by the short hairs
After you ate crow amd have gotten your access back, two fold tracks to go on. Legal will have to follow on any sort of follow up, and security leadership is going to have to go through a huge come to jesus moment in how they structure the department..
And in how employees are treated. How employees are treated is going to cover seperation of duties, more employees to share workloads, better work life balance, and a complete overhaul of management and their attitudes towards people
In a world where single points of failure aren't to be tolerated, they allowed a bad one to develop right there. Far from the only enterprise hanging by that thread.

So, would start w/ break-glass accounts, but if these are killed also, start opening tickets/making calls w/ vendors for cloud managed tools and look at restoring on prem tools from a recent snapshot, backup or immutable repository. So, this is why immutable needs to be a thing.

Disable accounts, reset sessions, block sign ins for that admin, reset password as well. Check logs for activity past 90 days maybe 180 if you have time?  PLUS look up a signed copy of the employee handbook and security policy by the admin and take legal action.

In order:
- wipe creds/revoke tokens/etc
- kick off major incident response, notify the person(s) necessary
- fire up the DC/PDC event logs and start sniffing.
- have a teammate run tickets with the tool providers (splunk etc)
- have manager run political football
- drink

