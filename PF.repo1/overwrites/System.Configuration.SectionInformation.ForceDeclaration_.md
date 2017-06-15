---
summary: Forces the associated configuration section to appear in the configuration file.
remarks: A configuration section is not written in a configuration file when it is inherited from a parent file. If you want the parent section to show in the child configuration file, you must set the <xref:System.Configuration.SectionInformation.ForceDeclaration%2A> to `true`. This makes a configuration file more portable from one computer to another. This also lets you make sure that the section exists even if you do not have control over parent configuration files.
uid: System.Configuration.SectionInformation.ForceDeclaration*
---
