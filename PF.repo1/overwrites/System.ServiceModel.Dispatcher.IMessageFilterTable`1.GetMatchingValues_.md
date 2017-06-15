---
summary: Adds the filter data of the filters that match the specified message or buffered message to a collection.
remarks: "Use this method when more than one filter is expected to match and only the matching filter data is required. These methods return a boolean that indicates whether matching filters were found and put any matching filter data into a collection.  \n  \n Note that the collection that contains the filter data is not cleared before the results are added. This allows you to accumulate all matches across multiple filter tables into a single collection.  \n  \n Use <xref:System.ServiceModel.Dispatcher.IMessageFilterTable%601.GetMatchingValues%2A> if the contents of the message body do not require examination. Use <xref:System.ServiceModel.Dispatcher.IMessageFilterTable%601.GetMatchingValues%2A> if the contents of the message body requires examination."
uid: System.ServiceModel.Dispatcher.IMessageFilterTable`1.GetMatchingValues*
---
