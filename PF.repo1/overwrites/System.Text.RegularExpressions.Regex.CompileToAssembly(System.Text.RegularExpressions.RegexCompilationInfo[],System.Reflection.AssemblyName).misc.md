---
uid: System.Text.RegularExpressions.Regex.CompileToAssembly(System.Text.RegularExpressions.RegexCompilationInfo[],System.Reflection.AssemblyName)
additional_notes.usage: *content
---

<p>If you are developing on a system that has [!INCLUDE[net_v45](~/includes/net-v45-md.md)] or its point releases installed, you target [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)], and you use the <xref href="System.Text.RegularExpressions.Regex.CompileToAssembly(System.Text.RegularExpressions.RegexCompilationInfo[],System.Reflection.AssemblyName)"></xref> method to create an assembly that contains compiled regular expressions. Trying to use one of the regular expressions in that assembly on a system that has [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)] throws an exception. To work around this problem, you can do either of the following:  
  
-   Build the assembly that contains the compiled regular expressions on a system that has [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)] instead of later versions installed.  
  
-   Instead of calling <xref href="System.Text.RegularExpressions.Regex.CompileToAssembly(System.Text.RegularExpressions.RegexCompilationInfo[],System.Reflection.AssemblyName)"></xref> and retrieving the compiled regular expression from an assembly, use either static or instance <xref href="System.Text.RegularExpressions.Regex"></xref> methods with the <xref href="System.Text.RegularExpressions.RegexOptions.Compiled"></xref> option when you instantiate a <xref href="System.Text.RegularExpressions.Regex"></xref> object or call a regular expression pattern matching method.</p>


