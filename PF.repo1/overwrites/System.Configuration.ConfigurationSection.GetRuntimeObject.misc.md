---
uid: System.Configuration.ConfigurationSection.GetRuntimeObject
additional_notes.overrides: *content
---

<p>You can override the <xref href="System.Configuration.ConfigurationSection.GetRuntimeObject"></xref> method to return a custom type at run time.  
  
 For example, to restrict runtime modification of the settings in the <xref href="System.Configuration.ConfigurationSection"></xref> class, you can override <xref href="System.Configuration.ConfigurationSection.GetRuntimeObject"></xref> and return a custom type that enforces restrictions on which settings can be modified, if any.  
  
 If the runtime object is internal only, the returned object cannot be used outside the assembly that defines it. One way to create an object that derives from <xref href="System.Configuration.ConfigurationSection"></xref> and can only be accessed by code in your assembly at run time is to create an internal runtime object that has a method that returns your <xref href="System.Configuration.ConfigurationSection"></xref> implementation.</p>


