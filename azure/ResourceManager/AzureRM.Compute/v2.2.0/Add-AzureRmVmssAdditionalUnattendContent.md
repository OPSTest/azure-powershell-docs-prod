---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: 44e1bf12-677d-4ffb-bd6f-b0bca2934a97
schema: 2.0.0
ms.assetid: BF0BCB7F-9C46-45BB-9324-5C8EB29CECC1
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/Add-AzureRmVmssAdditionalUnattendContent.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/Add-AzureRmVmssAdditionalUnattendContent.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureRmVmssAdditionalUnattendContent

## SYNOPSIS
Adds information to the unattended Windows Setup answer file.

## SYNTAX

```
Add-AzureRmVmssAdditionalUnattendContent [-VirtualMachineScaleSet] <VirtualMachineScaleSet>
 [[-PassName] <PassNames>] [[-ComponentName] <ComponentNames>] [[-SettingName] <SettingNames>]
 [[-Content] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmVmssAdditionalUnattendContent** cmdlet adds information to the unattended Windows Setup answer file.

## EXAMPLES

### Example 1: Add information to the unattended Windows Setup answer file
```
PS C:\>Add-AzureRmVmssAdditionalUnattendContent -VirtualMachineScaleSet $VMSS -ComponentName  $AUCComponentName -Content  $AUCContent -PassName $AUCPassName -SettingName  $AUCSetting
```

This command adds information to the unattended Windows Setup answer file.

## PARAMETERS

### -ComponentName
Specifies the name of the component to configure with the added content.
The only allowable value is Microsoft-Windows-Shell-Setup.

```yaml
Type: ComponentNames
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Content
Specifies the XML formatted content that is added to the unattend.xml file for the specified path and component.

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

### -PassName
Specifies the name of the pass that the content applies to.
The only allowable value is oobeSystem.

```yaml
Type: PassNames
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SettingName
Specifies the name of the setting to which the content applies.
The acceptable values for this parameter are::

- FirstLogonCommands
- AutoLogon

```yaml
Type: SettingNames
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VirtualMachineScaleSet
Specify the virtual machine **Scale Set** object.
You can use the New-AzureRmVmssConfig cmdlet to create the object.

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

## NOTES

## RELATED LINKS

[New-AzureRmVmssConfig](./New-AzureRmVmssConfig.md)


