---
uid: System.Xaml.Schema.XamlMemberInvoker.GetValue(System.Object)
additional_notes.overrides: *content
---

<p>The base implementation includes a call to the internal helper <code>ThrowIfUnknown</code>. This helper always throws for cases where a <xref href="System.Xaml.Schema.XamlMemberInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlMember"></xref>, which includes cases where the <xref href="System.Xaml.XamlMember.UnderlyingMember"></xref> of the <xref href="System.Xaml.XamlMember"></xref> is `null`.  
  
 The base implementation throws if <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingGetter"></xref> is `null`.  
  
 For static properties (<xref href="System.Reflection.MethodBase.IsStatic"></xref> is `true` per <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingGetter"></xref>) the default implementation calls <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> on <xref href="System.Xaml.Schema.XamlMemberInvoker.UnderlyingGetter"></xref> passing `null` as the first parameter and packaged <code>instance</code> in the second. For non-static properties, it calls <xref href="System.Reflection.MethodBase.Invoke(System.Object,System.Object[])"></xref> and forwards the <code>instance</code> as the first parameter and an empty package as the second parameter.</p>


