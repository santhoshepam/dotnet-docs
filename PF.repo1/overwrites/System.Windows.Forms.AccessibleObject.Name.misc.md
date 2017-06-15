---
uid: System.Windows.Forms.AccessibleObject.Name
additional_notes.overrides: *content
---

<p>All objects should support this property. An object's name should be intuitive so that users understand the object's meaning or purpose. Also, ensure that the `Name` property is unique relative to any sibling objects in the parent. Navigation within tables presents especially difficult problems for some users. Therefore, server developers should make table cell names as descriptive as possible. For example, you might create a cell name by combining the names of the row and column it occupies, such as "A1." However, it is generally better to use more descriptive names, such as "Karin, February." Many objects, such as icons, menus, check boxes, combo boxes, and other controls, have labels that are displayed to users. Any label displayed to users should be used for the object's <xref href="System.Windows.Forms.AccessibleObject.Name"></xref> property. For more information, see the <xref href="System.Windows.Forms.AccessibleObject.Name"></xref> Property.  
  
 If you are using menu or button text for the <xref href="System.Windows.Forms.AccessibleObject.Name"></xref> property, strip out the ampersands (&) that mark the keyboard access keys.</p>


