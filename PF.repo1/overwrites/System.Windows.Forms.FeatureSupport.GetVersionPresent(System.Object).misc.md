---
uid: System.Windows.Forms.FeatureSupport.GetVersionPresent(System.Object)
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Windows.Forms.FeatureSupport"></xref>, you must override this method. When you override this method, check that the class that you use for the <code>feature</code> parameter is the same as the class used for this parameter in the <xref href="System.Windows.Forms.FeatureSupport.IsPresent(System.String,System.String)"></xref> method. If the two <code>feature</code> parameters differ, you must also override <xref href="System.Windows.Forms.FeatureSupport.IsPresent(System.String,System.String)"></xref>.  
  
 See <xref href="System.Windows.Forms.OSFeature.GetVersionPresent(System.Object)"></xref> for an implementation of this method.</p>


