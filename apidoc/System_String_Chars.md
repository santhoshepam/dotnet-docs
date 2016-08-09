---
uid: System.String.Chars(System.Int32)
remarks: *content
---
The `index` parameter is zero-based.
This property returns the @System.Char object at the position specified by the `index` parameter. 
However, a Unicode character might be represented by more than one @System.Char. 
Use the @System.Globalization.StringInfo class to work with Unicode characters instead of @System.Char objects. 
For more information, see the "Char Objects and Unicode Characters" section in the @System.String class overview.

In C#, the @System.String.Chars(System.Int32) property is an indexer. In Visual Basic, it is the default property of the @System.String class. 
Each @System.Char object in the string can be accessed by using code such as the following.

```cs
string str1 = "Test";
for (int ctr = 0; ctr <= str1.Length - 1; ctr++ )
   Console.Write("{0} ", str1[ctr]);
// The example displays the following output:
//      T e s t  
```