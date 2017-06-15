---
uid: System.Web.UI.Adapters.ControlAdapter.OnLoad(System.EventArgs)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class and the adapter overrides the <xref href="System.Web.UI.Adapters.ControlAdapter.OnLoad(System.EventArgs)"></xref> method, the adapter must call the corresponding base class method, which in turn calls the <xref href="System.Web.UI.Control.OnLoad(System.EventArgs)"></xref> method. If <xref href="System.Web.UI.Control.OnLoad(System.EventArgs)"></xref> is not called, the <xref href="System.Web.UI.Control.Load"></xref> event will not be raised.</p>


