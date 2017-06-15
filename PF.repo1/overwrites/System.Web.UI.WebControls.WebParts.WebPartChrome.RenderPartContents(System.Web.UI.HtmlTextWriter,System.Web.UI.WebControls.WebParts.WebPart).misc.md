---
uid: System.Web.UI.WebControls.WebParts.WebPartChrome.RenderPartContents(System.Web.UI.HtmlTextWriter,System.Web.UI.WebControls.WebParts.WebPart)
additional_notes.overrides: *content
---

<p>You can optionally override the <xref href="System.Web.UI.WebControls.WebParts.WebPartChrome.RenderPartContents(System.Web.UI.HtmlTextWriter,System.Web.UI.WebControls.WebParts.WebPart)"></xref> method. If so, you can simply perform whatever rendering customizations you want for <code>webPart</code>, and then call its <xref href="System.Web.UI.Control.RenderControl(System.Web.UI.HtmlTextWriter)"></xref> method. If you also want to rely on the default rendering in the event of connection errors, call the base method first, and then customize the <code>writer</code> that is returned from the base method.</p>


