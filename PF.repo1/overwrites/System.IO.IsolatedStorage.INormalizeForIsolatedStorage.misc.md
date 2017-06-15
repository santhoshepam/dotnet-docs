---
uid: System.IO.IsolatedStorage.INormalizeForIsolatedStorage
additional_notes.overrides: *content
---

<p>Implement this interface when you are implementing custom evidence and need to determine if a store already exists. Serialized objects should not be used for comparisons in some instances, such as that of case sensitive strings. For example, www.MSN.com is equal to WWW.msn.com and will return a `true` when compared. To create an <xref href="System.IO.IsolatedStorage.INormalizeForIsolatedStorage"></xref> object, you need to implement the <xref href="System.IO.IsolatedStorage.INormalizeForIsolatedStorage.Normalize"></xref> method.</p>


---
uid: System.IO.IsolatedStorage.INormalizeForIsolatedStorage
additional_notes.usage: *content
---

<p>Call the methods of this interface to normalize the instance before making comparisons between an assembly's evidence and currently existing isolated stores.</p>


