---
uid: System.IO.IsolatedStorage.INormalizeForIsolatedStorage.Normalize
additional_notes.overrides: *content
---

<p>When you override this method and the object returned is a stream, it is assumed to be serialized and is compared directly to the serialized form of the evidence used to create existing stores. If the object returned is a string, it is considered the name of an isolated store and compared to the names of the existing stores.</p>


---
uid: System.IO.IsolatedStorage.INormalizeForIsolatedStorage.Normalize
additional_notes.usage: *content
---

<p>You typically call this method if you are writing a class derived from isolated storage and you need to check to see if isolated storage already exists for the current assembly.</p>


