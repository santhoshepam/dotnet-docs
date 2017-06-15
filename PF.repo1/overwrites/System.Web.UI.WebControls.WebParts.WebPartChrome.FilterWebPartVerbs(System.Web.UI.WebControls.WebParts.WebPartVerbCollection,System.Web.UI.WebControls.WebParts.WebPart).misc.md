---
uid: System.Web.UI.WebControls.WebParts.WebPartChrome.FilterWebPartVerbs(System.Web.UI.WebControls.WebParts.WebPartVerbCollection,System.Web.UI.WebControls.WebParts.WebPart)
additional_notes.overrides: *content
---

<p>If you create a custom <xref href="System.Web.UI.WebControls.WebParts.WebPartChrome"></xref> class, you can optionally override the <xref href="System.Web.UI.WebControls.WebParts.WebPartChrome.FilterWebPartVerbs(System.Web.UI.WebControls.WebParts.WebPartVerbCollection,System.Web.UI.WebControls.WebParts.WebPart)"></xref> method to filter out specific verbs from being rendered. The most common way to do this is to create a private method that checks the verbs in the <xref href="System.Web.UI.WebControls.WebParts.WebPart.Verbs"></xref> collection of a <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control and determines whether each verb should be rendered, based on criteria that you choose. Note that the base method provides a lot of default filtering criteria that would be difficult to reproduce if you completely override the method; if you only have a few special cases, you might want to call the base method first, and then pass the resulting collection through your own additional method to apply your custom filtering criteria.</p>


