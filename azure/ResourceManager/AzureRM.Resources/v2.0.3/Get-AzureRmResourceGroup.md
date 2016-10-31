---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: .\New-AzureRmResourceGroup.md
schema: 2.0.0
ms.assetid: 6282A378-C6F0-4A8E-BF68-DD5F68412205
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmResourceGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Get-AzureRmResourceGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
---

# Get-AzureRmResourceGroup

## SYNOPSIS
Gets resource groups.

## SYNTAX

### Lists the resource group based on the name. (Default)
```
Get-AzureRmResourceGroup [-Name <String>] [-Location <String>] [-ApiVersion <String>] [-Pre]
 [<CommonParameters>]
```

### Lists the resource group based on the Id.
```
Get-AzureRmResourceGroup [-Location <String>] [-Id <String>] [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmResourceGroup** cmdlet gets azure_2 resource groups in the current subscription.
You can get all resource groups, or specify a resource group by name or by other properties.
By default, this cmdlet gets all resource groups in the current subscription.

For more information about azure_2 resources and azure_2 resource groups, see the New-AzureRmResourceGroup cmdlet.

## EXAMPLES

### Example 1: Get a resource group by name
```
PS C:\>Get-AzureRmResourceGroup -Name "EngineerBlog"
```

This command gets the azure_2 resource group in your subscription named EngineerBlog.

### Example 2: Get all tags of a resource group
```
PS C:\>(Get-AzureRmResourceGroup -Name "ContosoRG").Tags
```

This command gets the resource group named ContosoRG, and displays the tags associated with that group.

## PARAMETERS

### -Id
Specifies the ID of the resource group to get.
Wildcard characters are not permitted.

```yaml
Type: String
Parameter Sets: Lists the resource group based on the Id.
Aliases: ResourceGroupId, ResourceId

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Specifies the location of the resource group to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the API version that is supported by the resource Provider.
You can specify a different version than the default version.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the resource group to get.
Wildcard characters are not permitted.

```yaml
Type: String
Parameter Sets: Lists the resource group based on the name.
Aliases: ResourceGroupName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### String
You can pipe input to the cmdlet by property name, but not by value.

## OUTPUTS

### Microsoft.Azure.Commands.ResourceManagement.PSResourceGroup
This cmdlet returns resource groups.

## NOTES

## RELATED LINKS

[New-AzureRmResourceGroup](xref:ResourceManager/AzureRM.Resources/v2.0.3/New-AzureRmResourceGroup.md)

[Remove-AzureRmResourceGroup](xref:ResourceManager/AzureRM.Resources/v2.0.3/Remove-AzureRmResourceGroup.md)

[Set-AzureRmResourceGroup](xref:ResourceManager/AzureRM.Resources/v2.0.3/Set-AzureRmResourceGroup.md)


