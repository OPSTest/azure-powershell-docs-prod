---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 7E6BD8E4-1C1E-451C-BA94-95202213474F
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Add-AzureRmVmssExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Add-AzureRmVmssExtension.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureRmVmssExtension

## SYNOPSIS
Adds an extension to the VMSS.

## SYNTAX

```
Add-AzureRmVmssExtension [-VirtualMachineScaleSet] <VirtualMachineScaleSet> [[-Name] <String>]
 [[-Publisher] <String>] [[-Type] <String>] [[-TypeHandlerVersion] <String>]
 [[-AutoUpgradeMinorVersion] <Boolean>] [[-Setting] <Object>] [[-ProtectedSetting] <Object>] [[-Id] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmVmssExtension** cmdlet adds an extension to the Virtual Machine Scale Set (VMSS).

## EXAMPLES

### Example 1: Add an extension to the VMSS
```
PS C:\>Add-AzureRmVmssExtension -VirtualMachineScaleSet $VMSS -Name $ExtName -Publisher $Publisher -Type $ExtType -TypeHandlerVersion $ExtVer -AutoUpgradeMinorVersion $True
```

This command adds an extension to the VMMS.

## PARAMETERS

### -AutoUpgradeMinorVersion
Indicates whether the extension version should be automatically updated to a newer minor version.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Id
Specifies an ID.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 9
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the extension that this cmdlet adds.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProtectedSetting
Specifies private configuration for the extension, as a string.
This cmdlet encrypts the private configuration.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 8
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Publisher
Specifies the name of the extension publisher.
The publisher provides a name when the publisher registers an extension.
This can use the Get-AzureRmVMImagePublisher cmdlet to get the publisher.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Setting
Specifies the public configuration, as a string, for the extension.
This cmdlet does not encrypt public configuration.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Type
Specifies the extension type.
You can use the Get-AzureRmVMExtensionImageType cmdlet to get the extension type.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TypeHandlerVersion
Specifies the version of the extension to use for this virtual machine.
You can use the Get-AzureRmVMExtensionImage cmdlet to get the version of the extension.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VirtualMachineScaleSet
Specify the VMSS object.
You can use the New-AzureRmVmssConfig to create the object.

```yaml
Type: VirtualMachineScaleSet
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

###  
This cmdlet does not generate any output.

## NOTES

## RELATED LINKS

[Remove-AzureRmVmssExtension](xref:ResourceManager/AzureRM.Compute/v2.3.0/Remove-AzureRmVmssExtension.md)

[Get-AzureRmVMImagePublisher](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVMImagePublisher.md)

[Get-AzureRmVMExtensionImageType](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVMExtensionImageType.md)

[Get-AzureRmVMExtensionImage](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVMExtensionImage.md)

[New-AzureRmVmssConfig](xref:ResourceManager/AzureRM.Compute/v2.3.0/New-AzureRmVmssConfig.md)

