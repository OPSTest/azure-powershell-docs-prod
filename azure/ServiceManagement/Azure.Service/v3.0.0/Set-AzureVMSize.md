---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 7f8a5fbb-7f93-40f7-a5d7-8e19fd65b65e
schema: 2.0.0
ms.assetid: BA63898A-23E5-4510-A198-E122E762AC7F
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureVMSize.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Set-AzureVMSize.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureVMSize

## SYNOPSIS
Sets the size of an Azure virtual machine.

## SYNTAX

```
Set-AzureVMSize [-InstanceSize] <String> -VM <IPersistentVM> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureVMSize** cmdlet updates the size of a virtual machine.
It has two parameters: *InstanceSize*, which is the new size of the virtual machine, and *VM*, which is a virtual machine object retrieved by using the Get-AzureVM cmdlet.
The result of **Set-AzureVMSize** can be piped to the Update-AzureVM cmdlet or stored in a variable for later use.
No actual change is made until **Update-AzureVM** is executed.

Note: This cmdlet will require the virtual machine to be re-provisioned and it might get a new IP address.

## EXAMPLES

### Example 1: Set the size of a virtual machine
```
PS C:\>Get-AzureVM -ServiceName "MySvc1" -Name "MyVM3" | Set-AzureVMSize "Small" | Update-AzureVM
```

This command updates a virtual machine to size "Small".

## PARAMETERS

### -InstanceSize
Specifies the size of the virtual machine.

The acceptable values for this parameter are:

--ExtraSmall
--Small
--Medium
--Large
--ExtraLarge
--A5
--A6
--A7

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VM
Specifies the persistent virtual machine object that this cmdlet sets the size of.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

[Get-AzureVM](xref:ServiceManagement/Azure.Service/v3.0.0/Get-AzureVM.md)

[Update-AzureVM](xref:ServiceManagement/Azure.Service/v3.0.0/Update-AzureVM.md)


