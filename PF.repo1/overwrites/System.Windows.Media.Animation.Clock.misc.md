---
uid: System.Windows.Media.Animation.Clock
additional_notes.overrides: *content
---

<p>Derived classes should implement <xref href="System.Windows.Media.Animation.Clock.GetCurrentTimeCore"></xref> if they want to modify how time flows for this clock. Derived classes can be made to do additional work when the clock repeats, skips, seeks, begins, pauses, resumes, or stops by overriding the <xref href="System.Windows.Media.Animation.Clock.DiscontinuousTimeMovement"></xref>, <xref href="System.Windows.Media.Animation.Clock.SpeedChanged"></xref>, and <xref href="System.Windows.Media.Animation.Clock.Stopped"></xref> methods.</p>


