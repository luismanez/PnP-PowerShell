#Get-SPOUserProfileProperty
Office365 only: Uses the tenant API to retrieve site information.

You must connect to the admin website (https://:<tenant>-admin.sharepoint.com) with Connect-SPOnline in order to use this command. 

##Syntax
```powershell
Get-SPOUserProfileProperty -Account <String[]>
```


##Detailed Description
Requires a connection to a SharePoint Tenant Admin site.

##Parameters
Parameter|Type|Required|Description
---------|----|--------|-----------
|Account|String[]|True|The account of the user, formatted either as a login name, or as a claims identity, e.g. i:0#.f|membership|user@domain.com|
##Examples

###Example 1
```powershell
PS:> Get-SPOUserProfileProperty -Account 'user@domain.com'
```
Returns the profile properties for the specified user

###Example 2
```powershell
PS:> Get-SPOUserProfileProperty -Account 'user@domain.com','user2@domain.com'
```
Returns the profile properties for the specified users
