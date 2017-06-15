---
uid: System.Windows.Forms.Control.OnResize(System.EventArgs)
additional_notes.overrides: *content
---

<p>When overriding <xref href="System.Windows.Forms.Control.OnResize(System.EventArgs)"></xref> in a derived class, be sure to call the base class's <xref href="System.Windows.Forms.Control.OnResize(System.EventArgs)"></xref> method so that registered delegates receive the event. The <xref href="System.Windows.Forms.Control.OnResize(System.EventArgs)"></xref> method can be called during construction, so if you override <xref href="System.Windows.Forms.Control.OnResize(System.EventArgs)"></xref> it can be called before the control constructor is called.</p>


