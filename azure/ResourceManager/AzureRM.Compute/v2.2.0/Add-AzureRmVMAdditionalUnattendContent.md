---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: ca32a23b-631a-4c8c-a045-719e7feef2cc
schema: 2.0.0
ms.assetid: C4F0EE47-E31F-4474-8E5D-0EF8DABB3433
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/Add-AzureRmVMAdditionalUnattendContent.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/Add-AzureRmVMAdditionalUnattendContent.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureRmVMAdditionalUnattendContent

## SYNOPSIS
Adds information to the unattended Windows Setup answer file.

## SYNTAX

```
Add-AzureRmVMAdditionalUnattendContent [-VM] <PSVirtualMachine> [[-Content] <String>]
 [[-SettingName] <SettingNames>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmVMAdditionalUnattendContent** cmdlet adds information to the unattended Windows Setup answer file.
Specify additional base 64 encoded .xml formatted information that this cmdlet adds to the unattend.xml file.

## EXAMPLES

### Example 1: Add content to unattend.xml
```
PS C:\>$AvailabilitySet = Get-AzureRmAvailabilitySet -ResourceGroupName "ResourceGroup11" -Name "AvailabilitySet03"
PS C:\> $VirtualMachine = New-AzureRmVMConfig -VMName "VirtualMachine07" -VMSize "Standard_A1" -AvailabilitySetID $AvailabilitySet.Id 
PS C:\> $Credential = Get-Credential
PS C:\> $VirtualMachine = Set-AzureRmVMOperatingSystem -VM $VirtualMachine  -Windows -ComputerName "Contoso26" -Credential $Credential
PS C:\> $AucContent = "<UserAccounts><AdministratorPassword><Value>" + "Password" + "</Value><PlainText>true</PlainText></AdministratorPassword></UserAccounts>";
PS C:\> $VirtualMachine = Add-AzureRmVMAdditionalUnattendContent -VM $VirtualMachine -Content $AucContent -SettingName "AutoLogon"
```

The first command gets the availability set named AvailablitySet03 in the resource group named ResourceGroup11, and then stores that object in the $AvailabilitySet variable.

The second command creates a virtual machine object, and then stores it in the $VirtualMachine variable.
The command assigns a name and size to the virtual machine.
The virtual machine belongs to the availability set stored in $AvailabilitySet.

The third command creates a credential object by using the Get-Credential cmdlet, and then stores the result in the $Credential variable.
The command prompts you for a user name and password.
For more information, type `Get-Help Get-Credential`.

The fourth command uses the **Set-AzureRmVMOperatingSystem** cmdlet to configure the virtual machine stored in $VirtualMachine.

The fifth command assigns content to the $AucContent variable.
The content includes a password.

The final command adds the content stored in $AucContent to the unattend.xml file.

## PARAMETERS

### -Content
Specifies base 64 encoded XML formatted content.
This cmdlet adds the content to the unattend.xml file.
The XML content must be less than 4 KB and must include the root element for the setting or feature that this cmdlet inserts.

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

### -SettingName
Specifies the name of the setting to which the content applies.
The acceptable values for this parameter are:

- FirstLogonCommands
- AutoLogon

```yaml
Type: SettingNames
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VM
Specifies the virtual machine object that this cmdlet modifies.
To obtain a virtual machine object, use the Get-AzureRmVM cmdlet.
Create a virtual machine object by using the New-AzureRmVMConfig cmdlet.

```yaml
Type: PSVirtualMachine
Parameter Sets: (All)
Aliases: VMProfile

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

[Get-AzureRmAvailabilitySet](xref:ResourceManager/AzureRM.Compute/v2.2.0/Get-AzureRmAvailabilitySet.md)

[Set-AzureRmVMOperatingSystem](xref:ResourceManager/AzureRM.Compute/v2.2.0/Set-AzureRmVMOperatingSystem.md)

[New-AzureRmVMConfig](xref:ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmVMConfig.md)


