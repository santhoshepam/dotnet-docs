---
summary: Asynchronously attempts to send an Internet Control Message Protocol (ICMP) echo message to a computer, and receive a corresponding ICMP echo reply message from that computer.
remarks: "These methods do not cause your application's main thread to block. If you want to block while waiting for the ICMP echo reply message, use the <xref:System.Net.NetworkInformation.Ping.Send%2A> methods.  \n  \n> [!NOTE]\n>  The IP address returned by any of the <xref:System.Net.NetworkInformation.Ping.SendAsync%2A> methods can originate from a malicious remote computer. Do not connect to the remote computer using this. Use DNS to determine the IP address of the machine to which you want to connect."
uid: System.Net.NetworkInformation.Ping.SendAsync*
---
