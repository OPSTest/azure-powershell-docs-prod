---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
ms.assetid: 6E190D23-9704-4BDF-8595-7F5946EB3D72
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.1.0/Get-AzureStorageAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.1.0/Get-AzureStorageAccount.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureStorageAccount

## SYNOPSIS
Gets the storage accounts for the current Azure subscription.

## SYNTAX

```
Get-AzureStorageAccount [[-StorageAccountName] <String>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureStorageAccount** cmdlet returns an object containing information about the storage accounts for the current subscription.
If the *StorageAccountName* parameter is specified, then only information about the specified storage account is returned.

## EXAMPLES

### Example 1: Return all storage accounts
```
PS C:\>Get-AzureStorageAccount
```

This command returns an object with all the storage accounts associated with the current subscription.

### Example 2: Return account information for a specified account
```
PS C:\>Get-AzureStorageAccount -StorageAccountName "ContosoStore01"
```

This command returns an object with only the ContosoStore01 account information.

### Example 3: Display a table of storage accounts
```
PS C:\>Get-AzureStorageAccount | Format-Table -AutoSize -Property @{Label="Name";Expression={$_.StorageAccountName}},"Label","Location"
```

This command returns an object with all the storage accounts associated with the current subscription, and outputs them as a table showing the account name, the account label, and the storage location.

## PARAMETERS

### -StorageAccountName
Specifies the name of a storage account.
If specified, this cmdlet returns only the specified storage account object.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
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

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

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

### ManagementOperationContext

## NOTES
* Type `help node-dev` to get help on Node.js development-related cmdlets. Type `help php-dev` to get help on PHP development-related cmdlets.

## RELATED LINKS

[New-AzureStorageAccount](xref:ServiceManagement/Azure.Service/v3.1.0/New-AzureStorageAccount.md)

[Set-AzureStorageAccount](xref:ServiceManagement/Azure.Service/v3.1.0/Set-AzureStorageAccount.md)

