---
uid: System.Random.Sample
additional_notes.overrides: *content
---

<p>Starting with the .NET Framework version 2.0, if you derive a class from <xref href="System.Random"></xref> and override the <xref href="System.Random.Sample"></xref> method, the distribution provided by the derived class implementation of the <xref href="System.Random.Sample"></xref> method is not used in calls to the base class implementation of the following methods:  
  
-   The <xref href="System.Random.NextBytes(System.Byte[])"></xref> method.  
  
-   The <xref href="System.Random.Next"></xref> method.  
  
-   The <xref href="System.Random.Next(System.Int32,System.Int32)"></xref> method, if (<code>maxValue</code> - <code>minValue</code>) is greater than <xref href="System.Int32.MaxValue"></xref>.  
  
 Instead, the uniform distribution provided by the base <xref href="System.Random"></xref> class is used. This behavior improves the overall performance of the <xref href="System.Random"></xref> class. To modify this behavior to call the implementation of the <xref href="System.Random.Sample"></xref> method in the derived class, you must also override the behavior of these three members. The example provides an illustration.</p>


