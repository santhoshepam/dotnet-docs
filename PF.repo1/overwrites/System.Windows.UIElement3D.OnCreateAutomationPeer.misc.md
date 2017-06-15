---
uid: System.Windows.UIElement3D.OnCreateAutomationPeer
additional_notes.overrides: *content
---

<p>The implementation of this method is typically to call the constructor of a specific <xref href="System.Windows.Automation.Peers.AutomationPeer"></xref> implementation, and return it as the return value.  
  
 All <xref href="System.Windows.UIElement3D"></xref> derived classes should implement this method in order to provide their own specific <xref href="System.Windows.Automation.Peers.AutomationPeer"></xref> implementations to the [!INCLUDE[TLA#tla_winclient](~/includes/tlasharptla-winclient-md.md)] infrastructure. For details on implementing this pattern, see <xref href="System.Windows.Automation.Peers.AutomationPeer"></xref>.</p>


