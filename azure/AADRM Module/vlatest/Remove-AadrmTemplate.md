---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=400630
schema: 2.0.0
ms.assetid: EAC26502-ECB3-43A0-B468-D166C1E4A9C4
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Remove-AadrmTemplate.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Remove-AadrmTemplate.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AadrmTemplate

## SYNOPSIS
Deletes a Rights Management rights policy template.

## SYNTAX

```
Remove-AadrmTemplate -TemplateId <Guid> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AadrmTemplate** cmdlet deletes an Azure Rights Management rights policy template.
You can delete only custom templates.
You can set default templates to an archived state but you cannot delete them.
After a template is deleted, content protected with that template might become inaccessible.
Users who are super users can continue to access content that was previously protected with a template that is now deleted.
For more information about super users, see Configuring super users for Azure Rights Management and discovery services or data recoveryhttps://docs.microsoft.com/rights-management/deploy-use/configure-super-users (https://docs.microsoft.com/rights-management/deploy-use/configure-super-users) on the Microsoft documentation site.

This cmdlet requires the template ID, which you can get with the Get-AadrmTemplate cmdlet.

This cmdlet performs the following operations:

- Displays the template properties.
- Warns that all content protected with this template may become inaccessible.
- Asks to confirm whether to proceed.
- Calls the service to remove the template with the specified GUID.

For more information about custom templates, see Configuring custom templates for Azure Rights Managementhttps://docs.microsoft.com/rights-management/deploy-use/configure-custom-templates (https://docs.microsoft.com/rights-management/deploy-use/configure-custom-templates) on the Microsoft documentation site.

## EXAMPLES

### Example 1: Delete a template
```
PS C:\>Remove-AadrmTemplate -TemplateId 36546649-4944-4462-a409-74373a67b6dd
```

This command deletes the specified template.

## PARAMETERS

### -TemplateId
Specifies the GUID of the Rights Management template.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmTemplate](./Add-AadrmTemplate.md)

[Export-AadrmTemplate](./Export-AadrmTemplate.md)

[Get-AadrmTemplate](./Get-AadrmTemplate.md)

[Import-AadrmTemplate](./Import-AadrmTemplate.md)


