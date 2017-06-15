---
uid: System.Windows.FrameworkElement.OnGotFocus(System.Windows.RoutedEventArgs)
additional_notes.overrides: *content
---

<p>If you intend to mark the event handled in the arguments, you should be aware of consequences on event handling in other parent elements in the element tree. Because this handler acts on an event with a bubbling routing, setting the focus to the current <code>sender</code> per the event arguments may not be appropriate. Focus might need to go to either a composite child element or to a parent element, depending on the compositing of certain controls. Therefore marking a focus event as handled is only recommended if the entirety of the visual tree that the event is routing through is part of compositing of a control that you authored.</p>


