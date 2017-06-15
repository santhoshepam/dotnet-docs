---
uid: System.Object.GetHashCode
additional_notes.overrides: *content
---

<p>A hash function is used to quickly generate a number (hash code) that corresponds to the value of an object. Hash functions are usually specific to each type and, for uniqueness, must use at least one of the instance fields as input. Hash codes should not be computed by using the values of static fields.  
  
 For classes derived from <xref href="System.Object"></xref>, the `GetHashCode` method can delegate to the base class <xref href="System.Object.GetHashCode"></xref> implementation only if the derived class defines equality to be reference equality. The default implementation of <xref href="System.Object.GetHashCode"></xref> for reference types returns a hash code that is equivalent to the one returned by the <xref href="System.Runtime.CompilerServices.RuntimeHelpers.GetHashCode(System.Object)"></xref> method. You can override <xref href="System.Object.GetHashCode"></xref> for immutable reference types. In general, for mutable reference types, you should override <xref href="System.Object.GetHashCode"></xref> only if:  
  
-   You can compute the hash code from fields that are not mutable; or  
  
-   You can ensure that the hash code of a mutable object does not change while the object is contained in a collection that relies on its hash code.  
  
 Otherwise, you might think that the mutable object is lost in the hash table. If you do choose to override <xref href="System.Object.GetHashCode"></xref> for a mutable reference type, your documentation should make it clear that users of your type should not modify object values while the object is stored in a hash table.  
  
 For value types, <xref href="System.ValueType.GetHashCode"></xref> provides a default hash code implementation that uses reflection. You should consider overriding it for better performance.  
  
 <block subset="none" type="note"><p>  
 For more information and examples that compute hash codes in a variety of ways, see the Examples section.  
  
</p></block>  
  
 A hash function must have the following properties:  
  
-   If two objects compare as equal, the <xref href="System.Object.GetHashCode"></xref> method for each object must return the same value. However, if two objects do not compare as equal, the <xref href="System.Object.GetHashCode"></xref> methods for the two objects do not have to return different values.  
  
-   The <xref href="System.Object.GetHashCode"></xref> method for an object must consistently return the same hash code as long as there is no modification to the object state that determines the return value of the object's <xref href="System.Object.Equals*"></xref> method. Note that this is true only for the current execution of an application, and that a different hash code can be returned if the application is run again.  
  
-   For the best performance, a hash function should generate an even distribution for all input, including input that is heavily clustered. An implication is that small modifications to object state should result in large modifications to the resulting hash code for best hash table performance.  
  
-   Hash functions should be inexpensive to compute.  
  
-   The <xref href="System.Object.GetHashCode"></xref> method should not throw exceptions.  
  
 For example, the implementation of the <xref href="System.String.GetHashCode"></xref> method provided by the <xref href="System.String"></xref> class returns identical hash codes for identical string values. Therefore, two <xref href="System.String"></xref> objects return the same hash code if they represent the same string value. Also, the method uses all the characters in the string to generate reasonably randomly distributed output, even when the input is clustered in certain ranges (for example, many users might have strings that contain only the lower 128 ASCII characters, even though a string can contain any of the 65,535 Unicode characters).  
  
 Providing a good hash function on a class can significantly affect the performance of adding those objects to a hash table. In a hash table with keys that provide a good implementation of a hash function, searching for an element takes constant time (for example, an O(1) operation). In a hash table with a poor implementation of a hash function, the performance of a search depends on the number of items in the hash table (for example, an O(<code>n</code>) operation, where <code>n</code> is the number of items in the hash table). A malicious user can input data that increases the number of collisions, which can significantly degrade the performance of applications that depend on hash tables, under the following conditions:  
  
-   When hash functions produce frequent collisions.  
  
-   When a large proportion of objects in a hash table produce hash codes that are equal or approximately equal to one another.  
  
-   When users input the data from which the hash code is computed.  
  
 Derived classes that override <xref href="System.Object.GetHashCode"></xref> must also override <xref href="System.Object.Equals(System.Object)"></xref> to guarantee that two objects considered equal have the same hash code; otherwise, the <xref href="System.Collections.Hashtable"></xref> type might not work correctly.</p>


