---
uid: System.Windows.Media.Animation.AnimationTimeline
additional_notes.overrides: *content
---

<p>To create a custom animation, override or implement the following members:  
  
-   <xref href="System.Windows.Freezable.CreateInstanceCore"></xref> – If your new class is concrete, you must override <xref href="System.Windows.Freezable.CreateInstanceCore"></xref> to return a new instance of your class.  
  
-   <xref href="System.Windows.Media.Animation.AnimationTimeline.GetCurrentValue(System.Object,System.Object,System.Windows.Media.Animation.AnimationClock)"></xref> – Override this method to return the current value of your animation. It takes three parameters: a default origin value, a default destination value, and an <xref href="System.Windows.Media.Animation.AnimationClock"></xref>. Use the <xref href="System.Windows.Media.Animation.AnimationClock"></xref> to obtain the current time or progress for the animation. You can choose whether to use the default origin and destination values.  
  
-   <xref href="System.Windows.Media.Animation.AnimationTimeline.IsDestinationDefault"></xref> – Override this property to indicate whether your animation uses the default destination value specified by the <xref href="System.Windows.Media.Animation.AnimationTimeline.GetCurrentValue(System.Object,System.Object,System.Windows.Media.Animation.AnimationClock)"></xref> method.  
  
-   <xref href="System.Windows.Media.Animation.AnimationTimeline.TargetPropertyType"></xref> – Override this property to indicate the <xref href="System.Type"></xref> of output your animation produces.  
  
 If the class does not use dependency properties to store its data or it requires extra initialization after creation, you might need to override additional methods; see the [Freezable Objects Overview](~/docs/framework/wpf/advanced/freezable-objects-overview.md) for more information.  
  
 For more information about creating custom animations, see the [Custom Animations Overview](~/docs/framework/wpf/graphics-multimedia/custom-animations-overview.md).</p>


