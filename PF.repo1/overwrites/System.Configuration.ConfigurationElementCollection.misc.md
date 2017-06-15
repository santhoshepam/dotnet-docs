---
uid: System.Configuration.ConfigurationElementCollection
additional_notes.overrides: *content
---

<p>You can use a programmatic or a declarative (attributed) coding model to create a custom configuration element.  
  
 The programmatic model requires that for each element attribute you create a property to get and set its value, and that you add it to the internal property bag of the underlying <xref href="System.Configuration.ConfigurationElement"></xref> base class.  
  
 The declarative model, also referred to as the attributed model, allows you to define an element attribute by using a property and configuring it with attributes. These attributes instruct the ASP.NET configuration system about the property types and their default values. ASP.NET can use reflection to obtain this information and then create the element property objects and perform the required initialization.</p>


