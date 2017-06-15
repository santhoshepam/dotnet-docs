---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.EndWebPartEditing
additional_notes.overrides: *content
---

<p>Developers who need to extend the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control might want to override this method in a derived class. One approach would be to call the base method and then add some additional custom handling, or you might want to completely customize the entire process of completing the editing of a control. For example, in the override method, you could call the base method first, and then add some code that determines what editing changes were made, and displays the list of changes back to the end user as a confirmation.</p>


