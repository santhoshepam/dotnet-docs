---
uid: System.String
---
> [!NOTE]
To view the .NET Framework source code for this type, see the [Reference Source](http://referencesource.microsoft.com/#mscorlib/system/string.cs#8281103e6f23cb5c). You can browse through the source code online, download the reference for offline viewing, and step through the sources (including patches and updates) during debugging; see [instructions](http://referencesource.microsoft.com/).

A string is a sequential collection of characters that is used to represent text. 
A @System.String object is a sequential collection of @System.Char?qualify=true objects that represent a string; 
a @System.Char?qualify=true object corresponds to a UTF-16 code unit. 
The value of the @System.String object is the content of the sequential collection of @System.Char?qualify=true objects, and that value is immutable (that is, it is read-only). 
For more information about the immutability of strings, see the [Immutability and the StringBuilder class)(#Immutability) section later in this topic. 
The maximum size of a @System.String object in memory is 2GB, or about 1 billion characters.

In this section:
         
- [Instantiating a String object](#Instantiation)
- [Char objects and Unicode characters](#Characters")
etc.

<a name="Instantiation"></a>
###Instantiating a String object

You can instantiate a @System.String object in the following ways:

- By assigning a string literal to a @System.String variable. This is the most commonly used method for creating a string. The following example uses assignment to create several strings. Note that in C#, because the backslash (\) is an escape character, literal backslashes in a string must be escaped or the entire string must be @-quoted. 

```csharp
string string1 = "This is a string created by assignment.";
Console.WriteLine(string1);
string string2a = "The path is C:\\PublicDocuments\\Report1.doc";
Console.WriteLine(string2a);
string string2b = @"The path is C:\PublicDocuments\Report1.doc";
Console.WriteLine(string2b);
// The example displays the following output:
//       This is a string created by assignment.
//       The path is C:\PublicDocuments\Report1.doc
//       The path is C:\PublicDocuments\Report1.doc    
```
              
- By calling a @System.String class constructor. The following example instantiates strings by calling several class constructors. Note that some of the constructors include pointers to character arrays or signed byte arrays as parameters. Visual Basic does not support calls to these constructors. For detailed information about @System.String constructors, see the @System.String.#ctor constructor summary.

etc.

<a name="Characters"></a>
### Char objects and Unicode characters

Each character in a string is defined by a Unicode scalar value, also called a Unicode code point or the ordinal (numeric) value of the Unicode character. 
Each code point is encoded by using UTF-16 encoding, and the numeric value of each element of the encoding is represented by a @System.Char object.

> [!NOTE]
Note that, because a @System.String instance consists of a sequential collection of UTF-16 code units, 
it is possible to create a @System.String object that is not a well-formed Unicode string. 
For example, it is possible to create a string that has a low surrogate without a corresponding high surrogate. 
Although some methods, such as the methods of encoding and decoding objects in the @System.Text namespace, may performs checks to ensure that strings are well-formed, 
@System.String class members do not ensure that a string is well-formed.

A single @System.Char object usually represents a single code point; that is, the numeric value of the @System.Char equals the code point. 
For example, the code point for the character "a" is U+0061. However, a code point might require more than one encoded element (more than one @System.Char object). 
The Unicode standard defines two types of characters that correspond to multiple @System.Char objects: 
graphemes, and Unicode supplementary code points that correspond to characters in the Unicode supplementary planes.

- A grapheme is represented by a base character followed by one or more combining characters. 
For example, the character ä is represented by a @System.Char object whose code point is U+0061 followed by a @System.Char object whose code point is U+0308. 
This character can also be defined by a single @System.Char object that has a code point of U+00E4. 
As the following example shows, a culture-sensitive comparison for equality indicates that these two representations are equal, although an ordinary ordinal comparison does not. 
However, if the two strings are normalized, an ordinal comparison also indicates that they are equal. 
(For more information on normalizing strings, see the [Normalization](#Normalization) section.)

```csharp
using System;
using System.Globalization;
using System.IO;

public class Example
{
   public static void Main()
   {
      StreamWriter sw = new StreamWriter(@".\graphemes.txt");
      string grapheme = "\u0061\u0308";
      sw.WriteLine(grapheme);

      string singleChar = "\u00e4";
      sw.WriteLine(singleChar);

      sw.WriteLine("{0} = {1} (Culture-sensitive): {2}", grapheme, singleChar, 
                   String.Equals(grapheme, singleChar, 
                                 StringComparison.CurrentCulture));
      sw.WriteLine("{0} = {1} (Ordinal): {2}", grapheme, singleChar, 
                   String.Equals(grapheme, singleChar, 
                                 StringComparison.Ordinal));
      sw.WriteLine("{0} = {1} (Normalized Ordinal): {2}", grapheme, singleChar, 
                   String.Equals(grapheme.Normalize(), 
                                 singleChar.Normalize(), 
                                 StringComparison.Ordinal));
      sw.Close(); 
   }
}
// The example produces the following output:
//       ä
//       ä
//       ä = ä (Culture-sensitive): True
//       ä = ä (Ordinal): False
//       ä = ä (Normalized Ordinal): True
```

etc.


<a name="Unicode"></a>

###Strings and The Unicode Standard
Characters in a string are represented by UTF-16 encoded code units, which correspond to @System.Char values. 
Each character in a string has an associated Unicode character category, which is represented in the .NET Framework by the @System.Globalization.UnicodeCategory enumeration. 
The category of a character or a surrogate pair can be determined by calling the @System.Globalization.CharUnicodeInfo.GetUnicodeCategory(System.Char)?qualify=true method.

The .NET Framework maintains its own table of characters and their corresponding categories, which ensures that a version of the .NET Framework running on different platforms returns identical character category information. 
The following table lists the versions of the .NET Framework and the versions of the Unicode Standard on which their character categories are based. 

| .NET Framework version | Version of the Unicode Standard     |
|------------------------|-------------------------------------|
| .NET Framework 1.1     | [The Unicode Standard, Version 4.0.0](http://www.unicode.org/versions/Unicode4.0.0/) |
| The .NET Framework 2.0 | [The Unicode Standard, Version 5.0.0](http://www.unicode.org/versions/Unicode5.0.0) |
| .NET Framework 3.5     | The Unicode Standard, Version 5.0.0 |
| .NET Framework 4       | The Unicode Standard, Version 5.0.0 |
| .NET Framework 4.5     | The Unicode Standard, Version 6.3.0 |
| .NET Framework 4.5.1   | The Unicode Standard, Version 6.3.0 |
| .NET Framework 4.5.2   | The Unicode Standard, Version 6.3.0 |
| .NET Framework 4.6     | The Unicode Standard, Version 6.3.0 |
| .NET Framework 4.6.1   | The Unicode Standard, Version 6.3.0 |
| .NET Framework 4.6.2   | The Unicode Standard, Version 8.0.0 |

<a name="EmbeddedNulls">>/a>
###Strings and embedded null characters
            
In the .NET Framework, a @System.String object can include embedded null characters, which count as a part of the string's length. 
However, in some languages such as C and C++, a null character indicates the end of a string;
it is not considered a part of the string and is not counted as part of the string's length. 
This means that the following common assumptions that C and C++ programmers or libraries written in C or C++ might make about strings are not necessarily valid 
when applied to @System.String objects:
              
- The value returned by the `strlen` or `wcslen` functions does not necessarily equal @System.String.Length?qualify=true.
- The string created by the `strcpy_s` or `wcscpy_s` functions is not necessarily identical to the string created by the @System.String.Copy(System.String)?qualify=true method.
                
You should ensure that native C and C++ code that instantiates @System.String objects, and code that is passed @System.String objects through platform invoke, 
do not assume that an embedded null character marks the end of the string.
Embedded null characters in a string are also treated differently when a string is sorted (or compared) and when a string is searched. 
Null characters are ignored when performing culture-sensitive comparisons between two strings, including comparisons using the invariant culture. 
They are considered only for ordinal or case-insensitive ordinal comparisons. 
On the other hand, embedded null characters are always considered when searching a string with methods such as @System.String.Contains(System.String), 
@System.String.StartsWith(System.String), and @System.String.IndexOf(System.String).