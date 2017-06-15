---
uid: System.Windows.Freezable.CloneCore(System.Windows.Freezable)
additional_notes.overrides: *content
---

<p>If you derive from <xref href="System.Windows.Freezable"></xref>, you may need to override this method. Reasons to override include the following:  
  
-   Your derived class has data that is not exposed via dependency properties.  
  
-   Your derived class must perform extra initialization work that cannot be accomplished by simply overriding <xref href="System.Windows.Freezable.CreateInstanceCore"></xref>. For example, this applies if your derived class implements <xref href="System.ComponentModel.ISupportInitialize"></xref>.  
  
 Classes that store all their data in dependency properties and that do not need to perform extra initialization work do not need to override <xref href="System.Windows.Freezable.CloneCore(System.Windows.Freezable)"></xref>.  
  
 It is essential that all implementations call the base implementation of this method. Implementations should only perform work that is not performed by the default implementation. The default implementation makes deep copies of all writable, locally set properties, including internal expressions.  
  
 If the object has data-bound dependency properties, the expressions are copied but might no longer resolve. For more information about cloning data-bound objects, see [Freezable Objects Overview](~/docs/framework/wpf/advanced/freezable-objects-overview.md). If the object has animated dependency properties, the base (non-animated) value of those properties is copied. Animations are not copied.  
  
 Note that unset properties are not copied, nor are read-only properties. If such a property has a default value that is a frozen <xref href="System.Windows.Freezable"></xref>, that property value remains frozen in the otherwise modifiable clone.  
  
 The following list summarizes the expected behavior for this method:  
  
-   The copy produced contains copies of all <xref href="System.Windows.Freezable"></xref> sub-objects.  
  
-   Unset and read-only properties are not copied.  
  
-   Expressions are copied.  
  
-   None of these sub-objects are frozen on creation.  
  
-   The copy itself is not frozen.  
  
-   Animations are not copied.  
  
-   Only property base values are copied, not current animated values.</p>


