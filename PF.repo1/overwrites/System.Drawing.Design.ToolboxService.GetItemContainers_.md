---
summary: Returns an <xref href="System.Collections.IList"></xref> containing all items on the toolbox.
remarks: "The items in the list must be <xref:System.Drawing.Design.ToolboxItemContainer> objects. If the toolbox implementation is organized in categories, this retrieves a combined list of all categories. The list must be read/write, as new items may be added to it.  \n  \n When the toolbox service adds a new item, it first calls the <xref:System.Drawing.Design.ToolboxService.CreateItemContainer%2A> method and then adds the new item to the <xref:System.Collections.IList> returned from the <xref:System.Drawing.Design.ToolboxService.GetItemContainers%2A> method.  \n  \n If a category name is provided, only the items in that category should be returned. If no category is specified, all items should be returned."
uid: System.Drawing.Design.ToolboxService.GetItemContainers*
---
