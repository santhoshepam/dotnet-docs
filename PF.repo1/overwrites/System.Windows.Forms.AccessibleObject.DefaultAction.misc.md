---
uid: System.Windows.Forms.AccessibleObject.DefaultAction
additional_notes.overrides: *content
---

<p>The default implementation returns the accessible object's default action if the object wraps a system control that has a default action; otherwise, it returns `null`. Only controls that perform actions should support this method. Not all objects have default actions, and some objects might have a default action that is related to its <xref href="System.Windows.Forms.AccessibleObject.Value"></xref> property, such as in the following examples: A selected check box has a default action of "Uncheck" and a value of "Checked." A cleared check box has a default action of "Check" and a value of "Unchecked." A button labeled "Print" has a default action of "Press," with no value. A static text control or an edit control that shows "Printer" has no default action, but would have a value of "Printer." An object's <xref href="System.Windows.Forms.AccessibleObject.DefaultAction"></xref> property should be a verb or a short verb phrase.</p>


