---
uid: System.Windows.Freezable.FreezeCore(System.Boolean)
additional_notes.overrides: *content
---

<p>
      <xref href="System.Windows.Freezable"></xref> implementers must override this method when the class contains data that is not stored using dependency properties.  
  
 A typical implementation would call base, then call the static <xref href="System.Windows.Freezable.Freeze(System.Windows.Freezable,System.Boolean)"></xref> method on all <xref href="System.Windows.Freezable"></xref> typed properties that the class contains, returning `true` only if all properties were frozen (or could have been frozen, in the case of specifying `true` for <code>isChecking</code>).</p>


