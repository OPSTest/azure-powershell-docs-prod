---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=722837
schema: 2.0.0
ms.assetid: 697EB0B3-9311-4F45-B1B7-489D7ABF911F
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Get-AadrmSuperUserGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Get-AadrmSuperUserGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AadrmSuperUserGroup

## SYNOPSIS
Gets the super user group for Rights Management.

## SYNTAX

```
Get-AadrmSuperUserGroup [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmSuperUserGroup** cmdlet gets the email address of the Azure Rights Management super user group for your organization.
This cmdlet does not get users that are individually assigned as super users with the Add-AadrmSuperUser cmdlet.

For more information about super users, see Configuring super users for Azure Rights Management and discovery services or data recoveryhttps://docs.microsoft.com/rights-management/deploy-use/configure-super-users (https://docs.microsoft.com/rights-management/deploy-use/configure-super-users) on the Microsoft documentation site.

## EXAMPLES

### Example 1: Get the super user group
```
PS C:\>Get-AadrmSuperUserGroup
```

This command gets the email address of the super user group for an organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.String
This operation returns the super user group email address as a **String**.
If no super user group exists, an empty **String** is returned.

## NOTES

## RELATED LINKS

[Add-AadrmSuperUser](./Add-AadrmSuperUser.md)

[Clear-AadrmSuperUserGroup](./Clear-AadrmSuperUserGroup.md)

[Set-AadrmSuperUserGroup](./Set-AadrmSuperUserGroup.md)


