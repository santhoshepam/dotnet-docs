---
uid: System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter.SaveAdapterState
additional_notes.overrides: *content
---

<p>The base implementation of <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter.SaveAdapterState"></xref> saves the current secondary UI mode in view state. You can override it to save other specific data from view state, but be sure to obtain the current state from the base class, and then combine it with your control-specific state in order to preserve the secondary UI mode across requests. For more information on managing view state, see [ASP.NET State Management Overview](http://msdn.microsoft.com/library/0218d965-5d30-445b-b6a6-8870e70e63ce).</p>


