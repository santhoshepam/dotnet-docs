---
uid: System.Console.OutputEncoding
additional_notes.usage: *content
---

<p>Of the Unicode encodings, the <xref href="System.Console"></xref> class supports UTF-8 encoding with the <xref href="System.Text.UTF8Encoding"></xref> class and, starting with the [!INCLUDE[net_v45](~/includes/net-v45-md.md)], it supports UTF-16 encoding with the <xref href="System.Text.UnicodeEncoding"></xref> class. UTF-32 encoding with the <xref href="System.Text.UTF32Encoding"></xref> class is not supported. Attempting to set the output encoding to UTF-32 throws an <xref href="System.IO.IOException"></xref>.  
  
 Note that successfully displaying Unicode characters to the console requires the following:  
  
-   The console must use a TrueType font, such as Lucida Console or Consolas, to display characters.  
  
-   A font used by the console must define the particular glyph or glyphs to be displayed. The console can take advantage of font linking to display glyphs from linked fonts if the base font does not contain a definition for that glyph.  
  
 For more information about support for Unicode encoding by the console, see the "Unicode Support for the Console" section in the <xref href="System.Console"></xref> class.</p>


