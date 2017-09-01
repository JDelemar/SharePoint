# SharePoint scripts/projects

Some SharePoint scripts/projects

The layout of this repo was inspired from NASA's [Open Source Catalog](https://github.com/nasa/Open-Source-Catalog) 

## Projects
|Name|Description|Keywords
|---|---|---
|[Dialogs And Notifications](https://github.com/JDelemar/SharePoint/tree/master/DialogsAndNotifications)|Use (and customize) SharePoint built in notifications to keep users informed of progress and/or status.|dialogs, notifications
|[1Template](https://github.com/JDelemar/SharePoint/tree/master/1Template)|Template for adding projects to this repo|template

## Retrieving a project
1. Clone the whole repository
   ```
   # clone the whole repository
   git clone https://github.com/JDelemar/SharePoint.git
   ```
   **OR**
   ```
   # do a sparse clone for a particular project (e.g. a project named "ProjectName")
   # create an empty repository
   mkdir SharePoint
   cd SharePoint
   git init
   git remote add -f origin https://github.com/JDelemar/SharePoint.git
   git config core.sparseCheckout true
   # define which files/folders to check out
   echo "ProjectName" >> .git/info/sparse-checkout
   ```
   `git pull origin master`  **OR** a shallow clone `git pull --depth=1 origin master`
   
2. Change directory to `ProjectName`

## TODO
|Name|Description
|---|---
|Get list fields|Get fields from list(s)
|Get list items|Get items from list(s)
|Get list views|Get views from list(s)
|Get list attachments|Get attachments from list(s)
|Make list|Make a SharePoint list
|Delete a list/items|Delete list and/or items
|Copy fields to new list|Creates a new list with designated fields with "better names" (e.g. no "_x0020_" in field names)
|Copy items to a list|Copies stored items to a list
|List view to editable grid view|Edit a list in a more presentable view
|Send email|Send email (bonus - include latest edit of version controlled multiline field)
|Custom form save|Make a form custom with validation and take over default save from EditForm.aspx
|User group management|Manage user groups
|Create subsite|Create a subsite with or without groups