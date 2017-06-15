---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.System#Web#UI#WebControls#WebParts#IPersonalizable#Save(System.Web.UI.WebControls.WebParts.PersonalizationDictionary)
additional_notes.overrides: *content
---

<p>One scenario in which developers would work with this method is if they are developing a custom personalization framework to use in place of the one provided by the Web Parts control set. In such cases, developers could inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreatePersonalization"></xref> method to return a custom implementation of a <xref href="System.Web.UI.WebControls.WebParts.WebPartPersonalization"></xref> object. The custom <xref href="System.Web.UI.WebControls.WebParts.WebPartPersonalization"></xref> object would call the implementation of the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.System#Web#UI#WebControls#WebParts#IPersonalizable#Save(System.Web.UI.WebControls.WebParts.PersonalizationDictionary)"></xref> method at the proper time to save the custom personalization data.</p>


