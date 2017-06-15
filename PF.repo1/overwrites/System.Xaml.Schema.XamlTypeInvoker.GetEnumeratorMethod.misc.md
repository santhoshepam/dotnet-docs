---
uid: System.Xaml.Schema.XamlTypeInvoker.GetEnumeratorMethod
additional_notes.overrides: *content
---

<p>The base implementation calls an internal helper method. That helper returns `null` for cases where a <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlType"></xref>, which includes cases where the <xref href="System.Xaml.XamlType.UnderlyingType"></xref> of the <xref href="System.Xaml.XamlType"></xref> is `null`. It also returns `null` for cases where <xref href="System.Xaml.XamlType.LookupCollectionKind"></xref> returns `None`.</p>


