---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400621
schema: 2.0.0
ms.assetid: 48A3F450-B87B-43DB-8723-8917FD5E0B7B
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Remove-AadrmSuperUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Remove-AadrmSuperUser.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AadrmSuperUser

## SYNOPSIS
Removes a super user from Rights Management.

## SYNTAX

```
Remove-AadrmSuperUser -EmailAddress <String> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AadrmSuperUser** cmdlet removes a user from the list of users who are individually granted super user privileges for your organization.
This cmdlet does not remove a group or a user from that a group that is assigned super user privileges by using the Set-AadrmSuperUserGroup cmdlet.
To add or remove super users, you must first enable the super user feature for Azure Rights Management by using the Enable-AadrmSuperUserFeature cmdlet.
For more information about super users, see the Get-AadrmSuperUser cmdlet.

## EXAMPLES

### Example 1: Remove a super user
```
PS C:\>Remove-AadrmSuperUser -EmailAddress "EvanNarvaez@Contoso.com"
```

This command removes an individually specified super user from Rights Management by specifying that user's email address.

## PARAMETERS

### -EmailAddress
Specifies the email address of a user or group.
The cmdlet removes the user or group identified by the email address that you specify.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmSuperUser](./Add-AadrmSuperUser.md)

[Get-AadrmSuperUser](./Get-AadrmSuperUser.md)

[Enable-AadrmSuperUserFeature](./Enable-AadrmSuperUserFeature.md)

[Set-AadrmSuperUserGroup](./Set-AadrmSuperUserGroup.md)


