---
uid: System.Windows.Freezable.CanFreeze
additional_notes.overrides: *content
---

<p>This method implementation uses the <xref href="System.Windows.Freezable.FreezeCore(System.Boolean)"></xref> method with <code>isChecking</code> set to `true` to determine whether a <xref href="System.Windows.Freezable"></xref> can be made unmodifiable. To modify the way this property behaves in a derived class, override the <xref href="System.Windows.Freezable.FreezeCore(System.Boolean)"></xref> method.</p>


