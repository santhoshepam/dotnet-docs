---
summary: Serves as a virtual method and converts information obtained by cache reflection into arguments for an asynchronous activity.
remarks: Custom activity authors can provide validation logic in an activity's <xref:System.Activities.AsyncCodeActivity%601.CacheMetadata%2A> override. Any exceptions that are thrown from <xref:System.Activities.AsyncCodeActivity%601.CacheMetadata%2A> are not treated as validation errors. These exceptions will escape from the call to <xref:System.Activities.Validation.ActivityValidationServices.Validate%2A> and must be handled by the caller.
uid: System.Activities.AsyncCodeActivity`1.CacheMetadata*
---
