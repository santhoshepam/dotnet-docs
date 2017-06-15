---
uid: System.Xaml.Schema.XamlTypeInvoker.CreateInstance(System.Object[])
additional_notes.overrides: *content
---

<p>The base implementation includes a call to the internal helper <code>ThrowIfUnknown</code>. This helper always throws for cases where a <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlType"></xref>, which includes cases where the <xref href="System.Xaml.XamlType.UnderlyingType"></xref> of the <xref href="System.Xaml.XamlType"></xref> is `null`.</p>


