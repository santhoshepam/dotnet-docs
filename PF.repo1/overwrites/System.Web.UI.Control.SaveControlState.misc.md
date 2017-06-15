---
uid: System.Web.UI.Control.SaveControlState
additional_notes.overrides: *content
---

<p>When control state is saved, a string object is returned to the client as a variable that is stored in an HTML `HIDDEN` element. Override this method to extract the state information to use in your control.  
  
 Control state is intended for small amounts of critical data, such as a page index or a keyword. Using control state for large amounts of data can adversely affect page performance. For more information, see [ASP.NET State Management Overview](http://msdn.microsoft.com/library/0218d965-5d30-445b-b6a6-8870e70e63ce).</p>


