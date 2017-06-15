---
uid: System.IComparable.CompareTo(System.Object)
additional_notes.overrides: *content
---

<p>For objects A, B and C, the following must be true:  
  
 <code>A.CompareTo(A)</code> must return zero.  
  
 If <code>A.CompareTo(B)</code> returns zero, then <code>B.CompareTo(A)</code> must return zero.  
  
 If <code>A.CompareTo(B)</code> returns zero and <code>B.CompareTo(C)</code> returns zero, then <code>A.CompareTo(C)</code> must return zero.  
  
 If <code>A.CompareTo(B)</code> returns a value other than zero, then <code>B.CompareTo(A)</code> must return a value of the opposite sign.  
  
 If <code>A.CompareTo(B)</code> returns a value <code>x</code> not equal to zero, and <code>B.CompareTo(C)</code> returns a value <code>y</code> of the same sign as <code>x</code>, then <code>A.CompareTo(C)</code> must return a value of the same sign as <code>x</code> and <code>y</code>.</p>


---
uid: System.IComparable.CompareTo(System.Object)
additional_notes.usage: *content
---

<p>Use the <xref href="System.IComparable.CompareTo(System.Object)"></xref> method to determine the ordering of instances of a class.</p>


