---
uid: System.ComponentModel.Design.IDesignerHost
additional_notes.usage: *content
---

<p>To obtain an implementation of <xref href="System.ComponentModel.Design.IDesignerHost"></xref> from a development environment, call <xref href="System.ComponentModel.Component.GetService(System.Type)"></xref> while your component is active in design mode, passing the type of <xref href="System.ComponentModel.Design.IDesignerHost"></xref> to request an <xref href="System.ComponentModel.Design.IDesignerHost"></xref> service interface.  
  
 <xref href="System.ComponentModel.Design.IDesignerHost"></xref> provides the following members related to designer state:  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.Loading"></xref> property indicates whether a designer or document is being loaded.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.Activated"></xref> event occurs when a designer is activated before display.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.Deactivated"></xref> event occurs when a designer is deactivated.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.LoadComplete"></xref> event occurs after a document is loaded.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.Activate"></xref> method activates the designer.  
  
 <xref href="System.ComponentModel.Design.IDesignerHost"></xref> provides the following members related to managing components:  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.Container"></xref> property indicates the container for the designer host.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.RootComponent"></xref> property indicates the base class for the root component.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.RootComponentClassName"></xref> property indicates the name of the class of the root component.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.CreateComponent(System.Type)"></xref> method creates the specified type of component.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.DestroyComponent(System.ComponentModel.IComponent)"></xref> method destroys the specified component.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.GetDesigner(System.ComponentModel.IComponent)"></xref> method gets the designer associated with a specified component.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.GetType(System.String)"></xref> method gets an instance of the type with the specified name.  
  
 <xref href="System.ComponentModel.Design.IDesignerHost"></xref> provides the following members related to managing transactions:  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.InTransaction"></xref> property indicates whether the designer is in a transaction.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.TransactionDescription"></xref> property indicates the current transaction description.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.TransactionClosed"></xref> event occurs when a transaction has been completed.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.TransactionClosing"></xref> event occurs when a transaction is about to be completed.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.TransactionOpened"></xref> event occurs when a transaction has begun.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.TransactionOpening"></xref> event occurs when a transaction is about to begin.  
  
-   The <xref href="System.ComponentModel.Design.IDesignerHost.CreateTransaction"></xref> method creates and returns a new transaction.</p>


