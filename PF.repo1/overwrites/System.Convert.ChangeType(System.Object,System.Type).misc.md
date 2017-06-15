---
uid: System.Convert.ChangeType(System.Object,System.Type)
additional_notes.usage: *content
---

<p>The <xref href="System.Convert.ChangeType(System.Object,System.Type)"></xref> method can convert an enumeration value to another type. However, it cannot convert another type to an enumeration value, even if the source type is the underlying type of the enumeration. To convert a type to an enumeration value, use a casting operator (in C#) or a conversion function (in Visual Basic). The following example illustrates the conversion to and from a <code>Continent</code> enumeration value.  
  
 [!code-csharp[System.Convert.ChangeType#5](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.convert.changetype/cs/changetype_enum2.cs#5)]
 [!code-vb[System.Convert.ChangeType#5](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.convert.changetype/vb/changetype_enum2.vb#5)]  
  
 The <xref href="System.Convert.ChangeType(System.Object,System.Type)"></xref> method can convert a nullable type to another type. However, it cannot convert another type to a value of a nullable type, even if <code>conversionType</code> is the underlying type of the <xref href="System.Nullable`1"></xref>.To perform the conversion, you can use a casting operator (in C#) or a conversion function (in Visual Basic). The following example illustrates the conversion to and from a nullable type.  
  
 [!code-csharp[System.Convert.ChangeType#7](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.convert.changetype/cs/changetype_nullable.cs#7)]
 [!code-vb[System.Convert.ChangeType#7](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.convert.changetype/vb/changetype_nullable.vb#7)]</p>


