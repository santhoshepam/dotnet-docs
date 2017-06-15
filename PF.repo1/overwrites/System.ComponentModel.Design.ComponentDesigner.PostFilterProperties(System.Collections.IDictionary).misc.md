---
uid: System.ComponentModel.Design.ComponentDesigner.PostFilterProperties(System.Collections.IDictionary)
additional_notes.overrides: *content
---

<p>You can directly filter the dictionary that is accessible through the <code>properties</code> parameter, or you can leave it unchanged. If you override this method, call the base implementation after you perform your own filtering. In addition, you must not remove items in the <xref href="System.ComponentModel.Design.ComponentDesigner.PostFilterProperties(System.Collections.IDictionary)"></xref> method. Instead, change attributes to hide items. You may also remove items in the <xref href="System.ComponentModel.Design.ComponentDesigner.PreFilterProperties(System.Collections.IDictionary)"></xref> method.</p>


