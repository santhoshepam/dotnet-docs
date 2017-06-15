---
uid: System.AppDomainManager.CreateDomain(System.String,System.Security.Policy.Evidence,System.AppDomainSetup)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.AppDomainManager"></xref> class and override the <xref href="System.AppDomainManager.CreateDomain(System.String,System.Security.Policy.Evidence,System.AppDomainSetup)"></xref> method, you can perform custom application domain initialization activities before calling the <xref href="System.AppDomainManager.CreateDomainHelper(System.String,System.Security.Policy.Evidence,System.AppDomainSetup)"></xref> method, or not call the helper method at all.  For example, you could modify the evidence passed in as <code>securityInfo</code>, update the fields of the associated <xref href="System.AppDomainSetup"></xref>, or reuse an exiting domain.</p>


