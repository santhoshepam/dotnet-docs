---
uid: System.Random
additional_notes.overrides: *content
---

<p>In the .NET Framework 1.0 and 1.1, a minimum implementation of a class derived from <xref href="System.Random"></xref> required overriding the <xref href="System.Random.Sample"></xref> method to define a new or modified algorithm for generating random numbers. The derived class could then rely on the base class implementation of the <xref href="System.Random.Next"></xref>, <xref href="System.Random.Next(System.Int32)"></xref>, <xref href="System.Random.Next(System.Int32,System.Int32)"></xref>, <xref href="System.Random.NextBytes(System.Byte[])"></xref>, and <xref href="System.Random.NextDouble"></xref> methods to call the derived class implementation of the <xref href="System.Random.Sample"></xref> method.  
  
 In the .NET Framework 2.0 and later, the behavior of the <xref href="System.Random.Next"></xref>, <xref href="System.Random.Next(System.Int32,System.Int32)"></xref>, and <xref href="System.Random.NextBytes(System.Byte[])"></xref> methods have changed so that these methods do not necessarily call the derived class implementation of the <xref href="System.Random.Sample"></xref> method. As a result, classes derived from <xref href="System.Random"></xref> that target the .NET Framework 2.0 and later should also override these three methods.</p>


---
uid: System.Random
additional_notes.usage: *content
---

<p>The implementation of the random number generator in the <xref href="System.Random"></xref> class isn't guaranteed to remain the same across major versions of the .NET Framework. As a result, you shouldn't assume that the same seed will result in the same pseudo-random sequence in different versions of the .NET Framework.</p>


