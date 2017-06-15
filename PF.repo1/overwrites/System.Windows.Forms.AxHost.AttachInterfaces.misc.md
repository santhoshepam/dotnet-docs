---
uid: System.Windows.Forms.AxHost.AttachInterfaces
additional_notes.overrides: *content
---

<p>Classes that extend <xref href="System.Windows.Forms.AxHost"></xref> should override this method. Within an overridden version of this method, the extending class should call <xref href="System.Windows.Forms.AxHost.GetOcx"></xref> to retrieve its own interface. In most cases, the <xref href="System.Windows.Forms.AxHost.GetOcx"></xref> method should not be called before this method is called.</p>


