---
uid: System.Xaml.XamlSchemaContext
additional_notes.overrides: *content
---

<p>In an <xref href="System.AppDomain"></xref>, a <xref href="System.Xaml.XamlSchemaContext"></xref> can be shared between multiple callers, which include both full and partial trust callers. This situation exists in frameworks such as WPF, which provide partial-trust access to XAML loading for portions of the WPF application model. The default <xref href="System.Xaml.XamlSchemaContext"></xref> implementation provides safeguards in this scenario by keeping all its properties and settings immutable. Derived implementations should also consider following this model of immutability for properties and settings of a XAML schema context.  
  
 The <xref href="System.Xaml.XamlSchemaContext"></xref> base class is designed so that lookups have no externally observable side effects. The types that are referenced by <xref href="System.Xaml.XamlSchemaContext"></xref> APIs in the base class, such as <xref href="System.Xaml.XamlType"></xref> or <xref href="System.Xaml.XamlMember"></xref>, also produce no side effects from lookups. All data that is needed to make a schema determination should be available from the construction and settings of the <xref href="System.AppDomain"></xref>. Notice that no lookup APIs rely on explicitly passed-in services; their input relies on string input only.  
  
 The <xref href="System.Xaml.XamlSchemaContext"></xref> base class, and <xref href="System.Xaml.XamlType"></xref> and <xref href="System.Xaml.XamlMember"></xref> are all thread safe in their base implementations. If you derive from <xref href="System.Xaml.XamlSchemaContext"></xref> or derive XAML type system classes such as <xref href="System.Xaml.XamlType"></xref> and <xref href="System.Xaml.XamlMember"></xref> , you can choose whether your classes will behave as thread safe.</p>


