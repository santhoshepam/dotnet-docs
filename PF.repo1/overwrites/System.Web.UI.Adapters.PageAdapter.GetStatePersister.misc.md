---
uid: System.Web.UI.Adapters.PageAdapter.GetStatePersister
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.PageAdapter"></xref> class, you can override the <xref href="System.Web.UI.Adapters.PageAdapter.GetStatePersister"></xref> method to return another derived page state persister if it is not feasible to maintain the combined state in a hidden field (for example, because of limited resources).  
  
 The <xref href="System.Web.UI.Adapters.PageAdapter.GetStatePersister"></xref> base class returns a <xref href="System.Web.UI.HiddenFieldPageStatePersister"></xref> object. You can use the <xref href="System.Web.UI.SessionPageStatePersister"></xref> class to maintain the page state in session state.</p>


