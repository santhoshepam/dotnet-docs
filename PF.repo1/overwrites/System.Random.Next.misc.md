---
uid: System.Random.Next
additional_notes.overrides: *content
---

<p>Starting with the .NET Framework version 2.0, if you derive a class from <xref href="System.Random"></xref> and override the <xref href="System.Random.Sample"></xref> method, the distribution provided by the derived class implementation of the <xref href="System.Random.Sample"></xref> method is not used in calls to the base class implementation of the <xref href="System.Random.Next"></xref> method. Instead, the uniform distribution returned by the base <xref href="System.Random"></xref> class is used. This behavior improves the overall performance of the <xref href="System.Random"></xref> class. To modify this behavior to call the <xref href="System.Random.Sample"></xref> method in the derived class, you must also override the <xref href="System.Random.Next"></xref> method.</p>


