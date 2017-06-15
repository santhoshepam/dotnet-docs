---
summary: Retrieves the current value of the specified property from an <xref href="System.Windows.Automation.AutomationElement"></xref>.
remarks: "The value returned by the <xref:System.Windows.Automation.AutomationElement.GetCurrentPropertyValue%2A> method is current at the time it is called. The value can subsequently change by other applications interacting with the [!INCLUDE[TLA#tla_ui](~/includes/tlasharptla-ui-md.md)].  \n  \n For some forms of [!INCLUDE[TLA2#tla_ui](~/includes/tla2sharptla-ui-md.md)], this method will incur cross-process performance overhead. Applications can concentrate overhead by caching properties and then retrieving them by using <xref:System.Windows.Automation.AutomationElement.GetCachedPropertyValue%2A>."
uid: System.Windows.Automation.AutomationElement.GetCurrentPropertyValue*
---
