---
uid: System.Xaml.Schema.XamlTypeInvoker.GetItems(System.Object)
additional_notes.overrides: *content
---

<p>The base implementation includes a call to the internal helper <code>ThrowIfUnknown</code>. This helper always throws for cases where a <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlType"></xref>, which includes cases where the <xref href="System.Xaml.XamlType.UnderlyingType"></xref> of the <xref href="System.Xaml.XamlType"></xref> is `null`.  
  
 The base implementation does not necessarily use its own <xref href="System.Xaml.Schema.XamlTypeInvoker.GetEnumeratorMethod"></xref> implementation. First, a cast of <code>instance</code> to <xref href="System.Collections.IEnumerable"></xref> is attempted. If this succeeds, a call to <xref href="System.Collections.IEnumerable.GetEnumerator"></xref> is made and the method returns that return value. Otherwise, the base implementation uses CLR <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> to invoke the underlying `GetEnumerator` method, as obtained from a call to <xref href="System.Xaml.Schema.XamlTypeInvoker.GetEnumeratorMethod"></xref> for this <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref>.</p>


