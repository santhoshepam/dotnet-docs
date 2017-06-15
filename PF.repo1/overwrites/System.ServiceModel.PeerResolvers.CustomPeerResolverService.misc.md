---
uid: System.ServiceModel.PeerResolvers.CustomPeerResolverService
additional_notes.overrides: *content
---

<p>Implementers of custom peer resolvers should derive from this class and override those specific functions for which they are providing custom implementations. Any custom peer resolver must minimally implement the <xref href="System.ServiceModel.PeerResolvers.IPeerResolverContract"></xref> interface.  
  
 Also, clients using a custom resolver must have some upper bound on client-server latency in order to successfully refresh their registration with the peer resolver service.</p>


