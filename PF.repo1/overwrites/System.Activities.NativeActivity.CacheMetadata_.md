---
summary: Creates and validates a description of the activity’s arguments, variables, child activities, and activity delegates.
remarks: Custom activity authors can provide validation logic in an activity's <xref:System.Activities.NativeActivity.CacheMetadata%2A> override. Any exceptions that are thrown from <xref:System.Activities.NativeActivity.CacheMetadata%2A> are not treated as validation errors. These exceptions will escape from the call to <xref:System.Activities.Validation.ActivityValidationServices.Validate%2A> and must be handled by the caller.
uid: System.Activities.NativeActivity.CacheMetadata*
---
