---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 2CF9D0A1-6708-468A-8E1E-03A284323322
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackVMRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackVMRole.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
---

# Get-WAPackVMRole

## SYNOPSIS

## SYNTAX

### Empty (Default)
```
Get-WAPackVMRole [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromCloudService
```
Get-WAPackVMRole [-Name] <String> [-CloudServiceName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromName
```
Get-WAPackVMRole [-Name] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see  Azure WAPack Cmdletshttp://msdn.microsoft.com/library/dn776450.aspx.
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type (get-module azure).version.

## EXAMPLES

### Example 1: Get a virtual machine role (created through the portal)
```
PS C:\>Get-WAPackVMRole -Name "ContosoVMRole01"
```

This command gets a virtual machine role which has been created through the portal named ContosoVMRole01.

### Example 2: Get a virtual machine role by using a name and a cloud service name
```
PS C:\>Get-WAPackVMRole -CloudServiceName "ContosoCloudService01" -Name "ContosoVMRole02"
```

This command gets a virtual machine role named ContosoVMRole02 which stand on a cloud service named ContosoCloudService01.

### Example 3: Get all virtual machine role
```
PS C:\>Get-WAPackVMRole
```

This command gets all existing virtual machine role.

## PARAMETERS

### -Name
Specifies the name of a virtual machine role.

```yaml
Type: String
Parameter Sets: FromCloudService, FromName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CloudServiceName
Specifies the cloud service name of virtual machine role.

```yaml
Type: String
Parameter Sets: FromCloudService
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
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

## OUTPUTS

## NOTES

## RELATED LINKS

[New-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/New-WAPackVMRole.md)

[Remove-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/Remove-WAPackVMRole.md)

[Set-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/Set-WAPackVMRole.md)


