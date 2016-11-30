---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 0CE86921-A610-4D5C-BF16-B447D96B59F2
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Set-WAPackVMRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Set-WAPackVMRole.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# Set-WAPackVMRole

## SYNOPSIS
Changes the instance count property of a virtual machine role.

## SYNTAX

```
Set-WAPackVMRole [-VMRole] <VMRole> [-InstanceCount] <Int32> [-PassThru] [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see  Azure WAPack Cmdletshttp://msdn.microsoft.com/library/dn776450.aspx.
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type (get-module azure).version.

The **Set-WAPackVMRole** cmdlet changes the instance count property of a virtual machine role.

## EXAMPLES

### Example 1: Specify the instance count for a virtual machine role
```
PS C:\>$VMRole = Get-WAPackVMRole -Name "ContosoVMRole01"
PS C:\>Set-WAPackVMRole -VMRole $VMRole -InstanceCount 3
```

The first command gets the virtual machine role named ContosoVMRole01 by using the Get-WAPackVMRole cmdlet, and then stores that object in the $VMRole variable.
The second and final command sets the new instance count of the virtual machine role stored in $VMRole to 3.

## PARAMETERS

### -VMRole
Specifies a virtual machine role.
To obtain a virtual machine role, use the Get-WAPackVMRole cmdlet.

```yaml
Type: VMRole
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InstanceCount
Specifies the instance count for a virtual machine role.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

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

[Get-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/Get-WAPackVMRole.md)

[New-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/New-WAPackVMRole.md)

[Remove-WAPackVMRole](xref:ServiceManagement/Azure.Compute/v3.0.0/Remove-WAPackVMRole.md)


