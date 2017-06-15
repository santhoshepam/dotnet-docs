---
uid: System.Xaml.Schema.XamlMemberInvoker.SetValue(System.Object,System.Object)
additional_notes.overrides: *content
---

<p>The base implementation includes a call to the internal helper <code>ThrowIfUnknown</code>. This helper always throws for cases where a <xref href="System.Xaml.Schema.XamlMemberInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlMember"></xref>, which includes cases where the <xref href="System.Xaml.XamlMember.UnderlyingMember"></xref> of the <xref href="System.Xaml.XamlMember"></xref> is `null`.  
  
 The base implementation throws if <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingSetter"></xref> is `null`.  
  
 For static properties (<xref href="System.Reflection.MethodBase.IsStatic"></xref> is `true` per <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingSetter"></xref>) the default implementation calls <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> on <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingSetter"></xref> passing `null` as the first parameter and packaging <code>instance</code> and <code>value</code> as the second parameter. For non-static properties, it calls <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> and forwards <code>instance</code> as first parameter and <code>value</code> as second parameter.</p>


