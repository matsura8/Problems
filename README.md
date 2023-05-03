# Problems
Just a place to note certain problems I've found with technology I am using. 

Example #1: Found this device in my firewall.

05: None 00.0: 0800 PIC (8259)
  [Created at misc.218]
  Unique ID: rdCR.8uRK7LxiIA2
  Hardware Class: unknown
  Model: "PIC"
  I/O Port: 0x00 (rw)
  I/O Port: 0x00 (rw)
  Config Status: cfg=new, avail=yes, need=no, active=unknown

Problem #2: Started digging through the hardware inventory of afforementioned firewall and found a company name that caught my attenttion. The company seems to specialize in wireless hardware using cellular or wifi signals. This is very curious since my firewall is a completely wired device. There is bluetooth connectivity to reach it, but that is supplied by a dongle and the dongle was removed during the hardware inventory. I find the company on Linked-In and when I go to the page the company has listed for itself, the page turns out to be an Indonesian Gambling site that doesn't provide a certificate. So, I can assume that my DNS is compromised, but I'm running my own DNS servers and they are setup to use DNSSEC and only allow secure updates. I am running AD on my domain and even have a subscription to Microsoft Defender for Cloud.

Using Shodan to look up owner of the servers, the trial ends at Cloudflare. It's always Cloudflare. Or RealTek.
