---
uid: System.Windows.Forms.AccessibleObject.Description
additional_notes.overrides: *content
---

<p>The default implementation returns the accessible object's description if the object wraps a system control; otherwise, it returns `null`. The description is typically used to provide greater context for low-vision or blind users. It can also be used for context searching or other applications. Servers need to support the <xref href="System.Windows.Forms.AccessibleObject.Description"></xref> property if the description is not obvious, or if it is redundant based on the object's <xref href="System.Windows.Forms.AccessibleObject.Name"></xref>, <xref href="System.Windows.Forms.AccessibleObject.Role"></xref>, <xref href="System.Windows.Forms.AccessibleObject.State"></xref>, and <xref href="System.Windows.Forms.AccessibleObject.Value"></xref> properties. For example, a button with "OK" does not need additional information, but a button that shows a picture of a cactus would. The <xref href="System.Windows.Forms.AccessibleObject.Name"></xref>, <xref href="System.Windows.Forms.AccessibleObject.Role"></xref>, and perhaps <xref href="System.Windows.Forms.AccessibleObject.Help"></xref> properties for the cactus button describe its purpose, but the <xref href="System.Windows.Forms.AccessibleObject.Description"></xref> property conveys information that is less tangible, like "A button that shows a picture of a cactus".</p>


