---
uid: System.Xaml.Schema.XamlTypeInvoker.AddToCollection(System.Object,System.Object)
additional_notes.overrides: *content
---

<p>The base implementation includes a call to the internal helper <code>ThrowIfUnknown</code>. This helper always throws for cases where a <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlType"></xref>, which includes cases where the <xref href="System.Xaml.XamlType.UnderlyingType"></xref> of the <xref href="System.Xaml.XamlType"></xref> is `null`.  
  
 Internally, the base implementation calls <xref href="System.Xaml.XamlType.IsCollection"></xref>, and throws if the result is `false`.  
  
 The base implementation does not necessarily use its own <xref href="System.Xaml.Schema.XamlTypeInvoker.GetAddMethod(System.Xaml.XamlType)"></xref> implementation. First, a cast of <code>instance</code> to <xref href="System.Collections.IList"></xref> is attempted. If this succeeds, a call to <xref href="System.Collections.IList.Add(System.Object)"></xref> is made and the method returns. Otherwise, the base implementation uses CLR <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> to invoke the underlying `Add` method, as obtained from a call to <xref href="System.Xaml.Schema.XamlTypeInvoker.GetAddMethod(System.Xaml.XamlType)"></xref> for this <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref>.  
  
 In the base implementation no exception is raised at this level if <code>item</code> is `null`. It is still possible that the underlying `Add` method will raise an exception when invoked. Other run time exceptions are possible if <xref href="System.Xaml.XamlType.ItemType"></xref> does not return a valid result.</p>


