---
summary: Adds a <xref href="System.Configuration.ConfigurationElement"></xref> to an <xref href="System.Configuration.ConfigurationElementCollection"></xref> instance when overridden in a derived class.
remarks: "Use the <xref:System.Configuration.ConfigurationElementCollection.BaseAdd%2A> method to add a new <xref:System.Configuration.ConfigurationElement> to the collection. Override in a derived class if custom behavior is required when the element is added.  \n  \n When adding, an element is considered a duplicate only if the keys are identical but the values are different. Elements with identical keys and values are accepted silently because the elements do not compete. However, an element with an identical key but a different value cannot be added because there is no logic to determine which of the competing values should be honored."
uid: System.Configuration.ConfigurationElementCollection.BaseAdd*
---
