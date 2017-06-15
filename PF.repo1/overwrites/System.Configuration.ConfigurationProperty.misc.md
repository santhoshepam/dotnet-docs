---
uid: System.Configuration.ConfigurationProperty
additional_notes.overrides: *content
---

<p>Every <xref href="System.Configuration.ConfigurationElement"></xref> object creates an internal <xref href="System.Configuration.ConfigurationPropertyCollection"></xref> collection of <xref href="System.Configuration.ConfigurationProperty"></xref> objects that represents either the element attributes or a collection of child elements.  
  
 Non-customizable information and functionality is contained by an <xref href="System.Configuration.ElementInformation"></xref> object provided by the <xref href="System.Configuration.ConfigurationElement.ElementInformation"></xref> property.  
  
 You can use a programmatic or a declarative (attributed) coding model to create a custom configuration element.  
  
-   Programmatic Model. This model requires that you create a property for each element attribute to get and/or set its value and add it to the internal property bag of the underlying <xref href="System.Configuration.ConfigurationElement"></xref> base class.  
  
-   Declarative Model. This simpler model, also called attributed model, allows you to define an element attribute by using a property and decorate it with attributes. These attributes instruct the ASP.NET configuration system about the property types and their default values. With this information, obtained through reflection, the ASP.NET configuration system creates the element property objects for you and performs the required initialization.</p>


