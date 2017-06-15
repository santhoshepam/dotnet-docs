---
uid: System.Runtime.Serialization.IDeserializationCallback
additional_notes.overrides: *content
---

<p>Implement the current interface as part of support for a method that is called when deserialization of the object graph is complete.  
  
 If an object needs to execute code on its child objects, it can delay this action, implement <xref href="System.Runtime.Serialization.IDeserializationCallback"></xref>, and execute the code only when it is called back on this interface.</p>


