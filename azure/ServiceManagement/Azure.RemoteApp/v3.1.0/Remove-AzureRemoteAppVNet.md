---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
ms.assetid: ED191A06-0C1D-486E-91F3-3CB61AA470A6
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.1.0/Remove-AzureRemoteAppVNet.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.1.0/Remove-AzureRemoteAppVNet.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_RemoteApp_v3_1_0_Remove_AzureRemoteAppVNet_md
---

# Remove-AzureRemoteAppVNet

## SYNOPSIS
Deletes an Azure RemoteApp virtual network.

## SYNTAX

```
Remove-AzureRemoteAppVNet -VNetName <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRemoteAppVNet** cmdlet deletes an Azure RemoteApp virtual network.

## EXAMPLES

### Example 1: Delete a specified virtual network
```
PS C:\>Remove-AzureRemoteAppVnet -VNetName "ContosoVNet"
```

This command deletes the virtual network named ContosoVNet

## PARAMETERS

### -VNetName
Specifies the name of the Azure RemoteApp virtual network to delete.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

[Get-AzureRemoteAppVNet](xref:ServiceManagement/Azure.RemoteApp/v3.1.0/Get-AzureRemoteAppVNet.md)

[Set-AzureRemoteAppVNet](xref:ServiceManagement/Azure.RemoteApp/v3.1.0/Set-AzureRemoteAppVNet.md)


