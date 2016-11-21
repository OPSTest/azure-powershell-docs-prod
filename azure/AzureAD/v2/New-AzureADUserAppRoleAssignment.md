---
external help file: azuread.help.xml
online version: https://blogs.technet.microsoft.com/enterprisemobility/2016/07/18/azuread-certificate-based-authentication-for-ios-and-android-now-in-preview/
schema: 2.0.0
updated_at: 11/21/2016 8:09 PM
ms.date: 11/21/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADUserAppRoleAssignment.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e79870303c4a5b18f88c61a5fe206bd45af8c480/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADUserAppRoleAssignment.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_New_AzureADUserAppRoleAssignment_md
---

# New-AzureADUserAppRoleAssignment

## SYNOPSIS
Assign a user to an application role.

## SYNTAX

```
New-AzureADUserAppRoleAssignment -ObjectId <String> -Id <String> -PrincipalId <String> -ResourceId <String>
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```
$OwnerAppRole = new-object Microsoft.Open.AzureAD.Model.AppRole -Property @{IsEnabled = $True; Description = "Owner Role"; AllowedMemberTypes = "user"; DisplayName = "MyApp Owner"; Id = [guid]::NewGuid(); Value="MyAppOwner"} 
$MyApp = New-AzureADApplication -DisplayName "MyApp" -IdentifierUris "http://MyNewApp.contoso.com" -AppRoles $OwnerAppRole
$ServicePrincipal = new-azureadserviceprincipal -AccountEnabled $true -AppId $MyApp.Id -ApproleAsignmentRequired $True -DisplayName "MyApp"
$User = get-azureaduser -top 1
New-AzureADUserAppRoleAssignment -ObjectId $user.ObjectId -PrincipalId $user.ObjectId -ResourceId $ServicePrincipal.ObjectId -Id $Role.Id
```

## PARAMETERS

### -ObjectId
The unique identifier of a user in Azure Active Directory (UPN or ObjectId)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -Id
The Id of the Role

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrincipalId
The PrincipalId

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceId
The object ID of the resource to which access is provided

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

