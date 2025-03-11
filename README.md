I built this automation to help illuminate SharePoint Sprawl. I have consulted for a number of firms that view SharePoint as the first and best place to build everything. Data is often exported from enterprise platforms (ERP, HR, Finance, CRM, etc.) so that "an application" can be built around that export in SharePoint. Maybe this solves a relatively small problem in the short term. In the long term it leads to enormous problems including, but limited to data security, data quality and lineage. It bypasses RBAC on the enterproise platforms, creates key person risk around the new so-called applications in SharePoint and only contributes to technical debt. 

Don't take my word. Use this automation to dump your SharePoint estate and see for yourself. Maybe everything is perfect in your world. Based on past experience, you may be in for a surprise. 

This Power Automate automation uses MS Graph to enumerate all of the SharePoint lists in the tenant. This automation does not use any premium features or Power Platform. The person running this automation does need read access to the MS Graph APIs to get the list of SharePoint sites. This person would typically be the Office 365 Admin. 

The automation will write details about each column to an Excel Spreadsheet. The details include: 
Site Name
List Name
Column Name
Column Data Type
Column Display Name
