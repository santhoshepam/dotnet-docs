---
uid: System.Windows.Freezable.CloneCurrentValueCore(System.Windows.Freezable)
additional_notes.overrides: *content
---

<p>If you derive from <xref href="System.Windows.Freezable"></xref>, you may need to override this method. Reasons to override include the following:  
  
-   Your derived class has data that is not exposed via dependency properties.  
  
-   Your derived class must perform extra initialization work that cannot be accomplished by simply overriding <xref href="System.Windows.Freezable.CreateInstanceCore"></xref>. For example, this applies if your derived class implements <xref href="System.ComponentModel.ISupportInitialize"></xref>.  
  
 Classes that store all their data in dependency properties and that do not need to perform extra initialization work do not need to override <xref href="System.Windows.Freezable.CloneCurrentValueCore(System.Windows.Freezable)"></xref>.  
  
 It is essential that all implementations call the base implementation of this method. Implementations should only perform work that is not performed by the default implementation. The default implementation makes deep copies of all writable, locally set properties. If the object contains dependency properties with expressions (such as a data binding), the current value of the expression is copied but not the expression itself.  
  
 If the object has animated dependency properties, the current animated value of those properties is copied, but the animations are not.  
  
 Note that unset properties are not copied, nor are read-only properties. If such a property has a default value that is a frozen <xref href="System.Windows.Freezable"></xref>, that property value remains frozen in the otherwise modifiable clone.  
  
 The following list summarizes the expected behavior for this method.  
  
-   The copy produced contains copies of all <xref href="System.Windows.Freezable"></xref> sub-objects.  
  
-   Unset and read-only properties are not copied.  
  
-   If a property is animated, its current value is copied, but the animation itself is not.  
  
-   None of these sub-objects are frozen on creation.  
  
-   The copy itself is not frozen.</p>


