---
uid: System.Windows.Markup.MarkupExtension.ProvideValue(System.IServiceProvider)
additional_notes.overrides: *content
---

<p>Common services returned by the default service provider that is typically available to a custom or existing <xref href="System.Windows.Markup.MarkupExtension"></xref> implementation include the following primary services.  
  
-   <xref href="System.Windows.Markup.IProvideValueTarget"></xref> reports the object reference and a property identifier from the context where the markup extension is used  
  
-   <xref href="System.Windows.Markup.IXamlTypeResolver"></xref> exposes a service that parallels the general XAML object writing behavior that can provide a <xref href="System.Type"></xref> based on a XAML type name. The name can optionally include a prefix for a mapped XAML namespace.  
  
-   <xref href="System.Xaml.IXamlSchemaContextProvider"></xref> exposes the active XAML schema context directly. From the reported <xref href="System.Xaml.XamlSchemaContext"></xref>, you can obtain XAML schema context information such as how assemblies are mapped for type support, preferred prefix in assemblies, lists of each <xref href="System.Xaml.XamlType"></xref> in an assembly, and so on.  
  
-   Other services available for more specialized markup extension scenarios include:  
  
    -   <xref href="System.Windows.Markup.IUriContext"></xref>  
  
    -   <xref href="System.Xaml.IAmbientProvider"></xref>  
  
    -   <xref href="System.Xaml.IDestinationTypeProvider"></xref>  
  
    -   <xref href="System.Xaml.IRootObjectProvider"></xref>  
  
    -   <xref href="System.Xaml.IXamlNameResolver"></xref>  
  
    -   <xref href="System.Xaml.IXamlNamespaceResolver"></xref>  
  
 Potentially, implementations of <xref href="System.Windows.Markup.MarkupExtension.ProvideValue(System.IServiceProvider)"></xref> can ignore the <code>serviceProvider</code> parameter. This is viable for some basic scenarios, where no context at all is required for returning a value.  
  
 In typical usage, the .NET Framework XAML Services and the implemented XAML object writers will provide a service provider to all value converter methods that are invoked during XAML processing. However, for robustness, you should provide code paths for null values both for the service provider itself and for any requested service. Null values might occur if your markup extension is applied in a circumstance where the typical service support provided by a XAML processor infrastructure is not available.  
  
 For more information on available services from the XAML service provider context and how to use them, see [Type Converters and Markup Extensions for XAML](~/docs/framework/xaml-services/type-converters-and-markup-extensions-for-xaml.md).  
  
 Implementations that require a certain service to be available in order to produce a useful <xref href="System.Windows.Markup.MarkupExtension.ProvideValue(System.IServiceProvider)"></xref> result are expected to throw exceptions if that service is not available. The recommended exception to throw is <xref href="System.InvalidOperationException"></xref>.  
  
 The implementation may also throw exceptions if one of the arguments that the custom markup extension needs in order to provide a value is null, is invalid for its data type, or does not contain a value that the markup extension is capable of processing. The recommended exception to throw is <xref href="System.InvalidOperationException"></xref>.</p>


