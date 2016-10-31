---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: efe9f766-cf6f-4793-b4ee-589d9659d393
schema: 2.0.0
ms.assetid: A2AF802A-C7E9-45DB-B399-C170ABB360D2
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Set-AzureRmPolicyDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Set-AzureRmPolicyDefinition.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
---

# Set-AzureRmPolicyDefinition

## SYNOPSIS
Modifies a policy definition.

## SYNTAX

### The policy definition name parameter set. (Default)
```
Set-AzureRmPolicyDefinition -Name <String> [-DisplayName <String>] [-Description <String>] [-Policy <String>]
 [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

### The policy definition Id parameter set.
```
Set-AzureRmPolicyDefinition -Id <String> [-DisplayName <String>] [-Description <String>] [-Policy <String>]
 [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmPolicyDefinition** cmdlet modifies a policy definition.

## EXAMPLES

### Example 1: Update the description of a policy definition
```
PS C:\>$PolicyDefinition = Get-AzureRmPolicyDefinition -Name "VMPolicyDefinition"
PS C:\> Set-AzureRmPolicyDefinition -Id $Policy.ResourceId -Description "Updated policy to not allow virtual machine creation"
```

The first command gets a policy definition named VMPolicyDefinition by using the Get-AzureRmPolicyDefinition cmdlet.
The command stores that object in the $PolicyDefinition variable.

The second command updates the description of the policy definition identified by the **ResourceId** property of $PolicyDefinition.

## PARAMETERS

### -Name
Specifies the name of the policy definition that this cmdlet modifies.

```yaml
Type: String
Parameter Sets: The policy definition name parameter set.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DisplayName
Specifies a new display name for the policy definition.

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

### -Description
Specifies a new description for the policy definition.

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

### -Policy
Specifies new policy rule for the policy definition.
You can specify the path of a .json file or a string that contains the policy in JavaScript Object Notation (JSON) format.

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
Specifies the version of the resource provider API to use.
If you do not specify a version, this cmdlet uses the latest available version.

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

### -Id
Specifies the fully qualified resource ID for the policy definition that this cmdlet modifies.

```yaml
Type: String
Parameter Sets: The policy definition Id parameter set.
Aliases: ResourceId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmPolicyDefinition](xref:ResourceManager/AzureRM.Resources/v3.2.0/Get-AzureRmPolicyDefinition.md)

[New-AzureRmPolicyDefinition](xref:ResourceManager/AzureRM.Resources/v3.2.0/New-AzureRmPolicyDefinition.md)

[Remove-AzureRmPolicyDefinition](xref:ResourceManager/AzureRM.Resources/v3.2.0/Remove-AzureRmPolicyDefinition.md)


