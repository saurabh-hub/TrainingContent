# DEMO: Office 365 Files
Use the completed lab project in the **Completed Solution** folder for this module as the demo.

Before running the demo you need to first create an app in Azure AD and update the project with the specific app information such as the client ID, client secret and Azure AD tenantID.

To do this, open the project in Visual Studio. Look at the lab and about half-way through **Exercise 1**, right after you create the project, pickup the steps to **Add the Connected Service**. Following these instructions will register the app in your Azure AD & update the `web.config` with the new app client ID and secret. 

The last step is to acquire your Azure AD tenantID (*the last step in Exercise 1*) and add that to the `web.config` in the app setting **tenantId**.

For the first demo, focus on the controller **FilesController** as it uses the OneDrive for Business native .NET SDK for the Office 365 Files API.

For the last demo, focus on the controller **OneDriveNewApiController** as it uses the new v2.0 REST API Microsoft is creating for OneDrive for Business that will mirror the API used in the OneDrive Consumer REST API for consistency.