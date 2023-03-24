# CVE-2023-23397-Report
An exploitation demo of Outlook Elevation of Privilege Vulnerability

CVE-2023-23397 is a critical EoP vulnerability in Microsoft Outlook that is triggered when an attacker sends a message with an extended MAPI property with a 
UNC path to an SMB (TCP 445) share on a threat actor-controlled server on an untrusted network. No user interaction is required. The threat actor is using a connection 
to the remote SMB server sends the user’s NTLM negotiation message, which the attacker can then relay for authentication against other systems that support 
NTLM authentication.
