---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400599
schema: 2.0.0
ms.assetid: E6136B57-7B45-4F74-8069-E23FB5D41E17
updated_at: 11/3/2016 6:06 AM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Disable-AadrmSuperUserFeature.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/c1e77f06e2ab5cf0e851dc3744ff83e69e84a33b/Azure%20Information%20Protection/AADRM/vlatest/Disable-AadrmSuperUserFeature.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Disable-AadrmSuperUserFeature

## SYNOPSIS
Disables the super user feature.

## SYNTAX

```
Disable-AadrmSuperUserFeature [<CommonParameters>]
```

## DESCRIPTION
The **Disable-AadrmSuperUserFeature** cmdlet disables the super user feature.
This action does not automatically remove the previously added users or group from the super user list, and they continue to be displayed when you run the Get-AadrmSuperUser or Get-AadrmSuperUserGroup cmdlets.
Therefore, if you enable the super user feature again, these users are automatically super users again, until you manually remove them.
If there are users in the current super list who must not be a super user if this feature is enabled again, remove them from the super user list before you disable the super user feature.
If these users are individually specified, remove them with the Remove-AadrmSuperUser cmdlet.
If they are a member of a group that you have specified to be a super user group, either remove those users from the specified super user group, or remove the super user group by using the Clear-AadrmSuperUserGroup cmdlet.

For information about the super user feature in Azure Rights Management, see Enable-AadrmSuperUserFeature.

## EXAMPLES

### Example 1: Disable super user feature
```
PS C:\>Disable-AadrmSuperUserFeature
```

This command disables the super user feature for your organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Clear-AadrmSuperUserGroup](xref:AADRM/vlatest/Clear-AadrmSuperUserGroup.md)

[Enable-AadrmSuperUserFeature](xref:AADRM/vlatest/Enable-AadrmSuperUserFeature.md)

[Get-AadrmSuperUserFeature](xref:AADRM/vlatest/Get-AadrmSuperUserFeature.md)

[Get-AadrmSuperUser](xref:AADRM/vlatest/Get-AadrmSuperUser.md)

[Get-AadrmSuperUserGroup](xref:AADRM/vlatest/Get-AadrmSuperUserGroup.md)

[Remove-AadrmSuperUser](xref:AADRM/vlatest/Remove-AadrmSuperUser.md)


