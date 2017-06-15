---
summary: Must be overridden in the derived class, and when implemented, gets the tracking profile for a specified workflow instance or workflow type.
remarks: A tracking service is responsible for managing the tracking profiles available for specific workflow types and specific workflow instances. You can implement this management in whatever manner you choose. For example, you can return the same <xref:System.Workflow.Runtime.Tracking.TrackingProfile> for every workflow <xref:System.Type> and workflow instance; or you can manage a sophisticated store of tracking profiles referenced by workflow instance, workflow <xref:System.Type>, and <xref:System.Version>.
uid: System.Workflow.Runtime.Tracking.TrackingService.GetProfile*
---
