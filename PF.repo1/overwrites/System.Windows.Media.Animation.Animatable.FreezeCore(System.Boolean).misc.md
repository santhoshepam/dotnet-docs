---
uid: System.Windows.Media.Animation.Animatable.FreezeCore(System.Boolean)
additional_notes.overrides: *content
---

<p>Classes that derive from <xref href="System.Windows.Media.Animation.Animatable"></xref> must override this method when the class contains data that is not stored using dependency properties.  
  
 A typical implementation would call the base implementation, then call the static <xref href="System.Windows.Freezable.Freeze"></xref> method on all <xref href="System.Windows.Freezable"></xref> typed properties that the class contains, returning `true` only if all properties were frozen (or could have been frozen, in the case of passing through a `false` value for <code>isChecking</code>).</p>


