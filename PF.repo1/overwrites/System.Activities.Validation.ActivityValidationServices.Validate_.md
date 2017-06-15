---
summary: Verifies that a workflow activity is correctly configured according to the validation logic. This logic can be the <xref href="System.Activities.CodeActivity.CacheMetadata(System.Activities.CodeActivityMetadata)"></xref> method of the activities to validate, or build and policy constraints.
remarks: Custom activity authors can provide validation logic in an activity's <xref:System.Activities.CodeActivity.CacheMetadata%2A> override. Any exceptions that are thrown from <xref:System.Activities.CodeActivity.CacheMetadata%2A> are not treated as validation errors. These exceptions will escape from the call to <xref:System.Activities.Validation.ActivityValidationServices.Validate%2A> and must be handled by the caller.
uid: System.Activities.Validation.ActivityValidationServices.Validate*
---
