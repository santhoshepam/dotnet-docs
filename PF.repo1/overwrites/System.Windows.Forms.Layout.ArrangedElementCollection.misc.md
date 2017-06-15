---
uid: System.Windows.Forms.Layout.ArrangedElementCollection
thread_safety: *content
---

Public `static` (`Shared` in Visual Basic) members of this type are thread safe. Instance members are not guaranteed to be thread safe.  
  
 An <xref href="System.Windows.Forms.Layout.ArrangedElementCollection"></xref> can support multiple readers concurrently, as long as the collection is not modified. The <xref href="System.Windows.Forms.Layout.ArrangedElementCollection.GetEnumerator"></xref> method returns an <xref href="System.Collections.IEnumerator"></xref> that can be used to access elements.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads could still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


