---
uid: System.Enum.ToString
additional_notes.usage: *content
---

<p>If multiple enumeration members have the same underlying value and you attempt to retrieve the string representation of an enumeration member's name based on its underlying value, your code should not make any assumptions about which name the method will return. For example, the following enumeration defines two members, <code>Shade.Gray</code> and <code>Shade.Grey</code>, that have the same underlying value.  
  
 [!code-csharp[System.Enum.ToString#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.enum.tostring/cs/tostringbyvalue1.cs#1)]
 [!code-vb[System.Enum.ToString#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.enum.tostring/vb/tostringbyvalue1.vb#1)]  
  
 The following method call attempts to retrieve the name of a member of the <code>Shade</code> enumeration whose underlying value is 1. The method can return either "Gray" or "Grey", and your code should not make any assumptions about which string will be returned.  
  
 [!code-csharp[System.Enum.ToString#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.enum.tostring/cs/tostringbyvalue1.cs#2)]
 [!code-vb[System.Enum.ToString#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.enum.tostring/vb/tostringbyvalue1.vb#2)]</p>


