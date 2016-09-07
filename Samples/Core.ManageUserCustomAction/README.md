# Manage UserCustomAction using SharePoint Add-In #

### Summary ###
The Core.ManageUserCustomAction sample shows how to manage UserCustomActions Objects using a Form interface where is possible to include/edit/delete UserCustomActions. This sample app extends the Out of the Box SharePoint Object "UserCustomAction" with a basic user interface Form with pre-filled data needed to support the object that allows Power Users to manage custom actions like "Scriptlink", "Ribbons" and "Custom Actions" in the Hosted Site.

### Applies to ###
-  Office 365 Multi Tenant (MT)
-  Office 365 Dedicated (D)
-  SharePoint 2013 on-premises

### Prerequisites ###
None

### Solution ###
Solution | Author(s)
---------|----------
Core.ManageUserCustomAction| **André Lage**

### Version history ###
Version  | Date | Comments
---------| -----| --------
1.0  | May 26th 2015 | Initial release

### Disclaimer ###
**THIS CODE IS PROVIDED *AS IS* WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING ANY IMPLIED WARRANTIES OF FITNESS FOR A PARTICULAR PURPOSE, MERCHANTABILITY, OR NON-INFRINGEMENT.**


----------

# Instalation #
The Solution is an SharePoint Add-In that can be deployed in the app catalog site of the Tenant and then install in the SharePoint Site using "Add an app" Option.

## Manage UserCustomAction SharePoint Add-In ##

The app manages SharePoint Site "SP.Web" UserCustomActions from and Custom Form created in an SharePoint Add-In.

![Add-in UI](http://i.imgur.com/sfvGTuv.png)

The idea is integrate Power User "Business decision" and Developer work using existing SharePoint Objects "UserCustomAction" with user friendy interface to remove the current complexity of this objects management.
This sample explains how is possible to create a split between Power Users and Developer's.
### Developer ###
- Creation of Html, JS or CSS files deployed in Assets Libraries to support custom solutions that are included by the Power Users using UserCustomActions.

### Power Users ###
- Integration of Developer's work into SharePoint Site, using Scriptlinks or Custom Ribbons with actions.

![Process picture on the action management](http://i.imgur.com/J6fzFru.png)

## Manage UserCustomAction SharePoint Add-In functionalities ##

### Form Actions ###
- Clean Form (cleanup of fields)
- New UserCustomAction
- Edit UserCustomAction
- Delete UserCustomAction

### Autofill fields: ###
- UserCustomActions Tokens (Image Url, ScriptBlock, ScriptSrc and Url Action fields)
- ListTemplates Id (RegistrationId field)
- Web Content Types and List Content Types (RegistrationId field)
- ProgId  (RegistrationId field)
- FileTypes (RegistrationId field)
- SharePoint Base Permissions (Rights field)

### Picker Control: ###
- List ID (RegistrationId field "Browse" button allow to select List Id)
- File Picker (Image Url and ScriptSrc "Browse" button allow to select file in SharePoint Site)

### Leasons Learn: ###
- Creation of good UI and UX is critical for better acceptance of an app.
- Creation of Log List to support errors generated by the app.
- Creation of Help or/and tutorial on how to work with the app.
- Creation of Recycle List to store deleted SharePoint Object "UserCustomActions" base in JSON, by default this SharePoint Objects are not stored in the Out of the Box recycled bin.
- Creation of Resource files or [Language].js files to support a multilanguage app.

<img src="https://telemetry.sharepointpnp.com/pnp/samples/Core.ManageUserCustomAction" />