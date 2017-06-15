---
uid: System.Windows.Forms.FeatureSupport.IsPresent(System.Object,System.Version)
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Windows.Forms.FeatureSupport"></xref>, you must override the <xref href="System.Windows.Forms.FeatureSupport.GetVersionPresent(System.String,System.String)"></xref> method. When you override this method, check that the class that you use for the <code>feature</code> parameter is the same as the class used for this parameter in the <xref href="System.Windows.Forms.FeatureSupport.IsPresent(System.String,System.String)"></xref> method. If the two <code>feature</code> parameters differ, you must also override <xref href="System.Windows.Forms.FeatureSupport.IsPresent(System.String,System.String)"></xref>.</p>


