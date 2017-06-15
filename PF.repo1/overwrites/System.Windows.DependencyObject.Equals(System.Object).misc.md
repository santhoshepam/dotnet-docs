---
uid: System.Windows.DependencyObject.Equals(System.Object)
additional_notes.overrides: *content
---

<p>
      <xref href="System.Windows.DependencyObject"></xref> overrides and then seals two basic <xref href="System.Object"></xref> methods: <xref href="System.Windows.DependencyObject.Equals(System.Object)"></xref> and <xref href="System.Windows.DependencyObject.GetHashCode"></xref>. The overrides call the <xref href="System.Object"></xref> implementations, resulting in an object equality behavior. The purpose of these deliberate overrides is to prevent derived classes from trying to define a value equality for a <xref href="System.Windows.DependencyObject"></xref>. Value equalities for <xref href="System.Windows.DependencyObject"></xref> will never be accurate because of the innate property value-changing capabilities of a <xref href="System.Windows.DependencyObject"></xref> and its dependency properties. This includes fundamental [!INCLUDE[TLA2#tla_winclient](~/includes/tla2sharptla-winclient-md.md)] features such as data binding and the [!INCLUDE[TLA2#tla_winclient](~/includes/tla2sharptla-winclient-md.md)] property system.</p>


