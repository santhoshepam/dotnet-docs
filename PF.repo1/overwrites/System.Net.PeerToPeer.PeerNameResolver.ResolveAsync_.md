---
summary: These methods begin an asynchronous resolution operation for the specified <xref href="System.Net.PeerToPeer.PeerName"></xref> in all clouds known to the calling peer.
remarks: "For every <xref:System.Net.PeerToPeer.PeerNameResolver.Resolve%2A> method, there is an equivalent <xref:System.Net.PeerToPeer.PeerNameResolver.ResolveAsync%2A> method, which is used when asynchronous processing is required.  They are identical in the parameters they are passed, except that ResolveAsync includes a system token in its parameter list for event handling.  \n  \n If a parameter mismatch occurs between the Resolve method and the ResolveAsync method, and the <xref:System.Net.PeerToPeer.Cloud> parameter is not supplied, the method uses the <xref:System.Net.PeerToPeer.Cloud.Available> shortcut to fill in cloud parameters."
uid: System.Net.PeerToPeer.PeerNameResolver.ResolveAsync*
---
