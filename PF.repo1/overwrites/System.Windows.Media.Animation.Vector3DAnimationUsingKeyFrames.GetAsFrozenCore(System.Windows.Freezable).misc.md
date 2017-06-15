---
uid: System.Windows.Media.Animation.Vector3DAnimationUsingKeyFrames.GetAsFrozenCore(System.Windows.Freezable)
additional_notes.overrides: *content
---

<p>A subclass should override this method if it has data that is not exposed via dependency properties or it performs extra work during construction.  
  
 The default implementation makes clones of all writable, unfrozen, locally set properties. Note that the properties' base values are copied, not their current values. The default implementation does not clone read-only dependency properties or frozen values.  
  
 If you do override this method, you must call the <xref href="System.Windows.Media.Animation.Vector3DAnimationUsingKeyFrames"></xref> implementation.</p>


