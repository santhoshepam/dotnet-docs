---
uid: System.Xaml.Schema.XamlTypeInvoker.GetAddMethod(System.Xaml.XamlType)
additional_notes.overrides: *content
---

<p>The base implementation returns `null` for cases where a <xref href="System.Xaml.Schema.XamlTypeInvoker"></xref> is based on an unknown <xref href="System.Xaml.XamlType"></xref>, which includes cases where the <xref href="System.Xaml.XamlType.UnderlyingType"></xref> of the <xref href="System.Xaml.XamlType"></xref> is `null`. It also returns `null` if <xref href="System.Xaml.XamlType.ItemType"></xref> is `null`.  
  
 XAML collections potentially have more than one `Add` method, because a XAML collection can potentially support more than one content type (see <xref href="System.Xaml.XamlType.AllowedContentTypes"></xref>, or see <xref href="System.Windows.Markup.ContentWrapperAttribute"></xref> for information about one implementation of this concept in WPF). The default implementation uses internal logic to return the best match based on the signatures and the type of the supplied <code>contentType</code>.</p>


