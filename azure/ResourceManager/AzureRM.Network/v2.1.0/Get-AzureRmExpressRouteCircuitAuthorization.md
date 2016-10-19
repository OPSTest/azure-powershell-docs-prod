---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureRmExpressRouteCircuitAuthorization.md
schema: 2.0.0
ms.assetid: A3CE99B1-CA65-4241-8018-4E80226AB610
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmExpressRouteCircuitAuthorization.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmExpressRouteCircuitAuthorization.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmExpressRouteCircuitAuthorization

## SYNOPSIS
Gets information about ExpressRoute circuit authorizations.

## SYNTAX

```
Get-AzureRmExpressRouteCircuitAuthorization [-Name <String>] -ExpressRouteCircuit <PSExpressRouteCircuit>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmExpressRouteCircuitAuthorization** cmdlet gets information about the authorizations assigned to an ExpressRoute circuit.
ExpressRoute circuits connect your on-premises network to the Microsoft cloud by using a connectivity provider instead of the public Internet.
The owner of an ExpressRoute circuit can create as many as 10 authorizations for each circuit; these authorizations generate an authorization key that can be used by a virtual network owner to connect his or her network to the circuit (one authorization per virtual network).
Authorization keys, as well as other information about the authorization, can be viewed at any time by running **Get-AzureRmExpressRouteCircuitAuthorization**.

## EXAMPLES

### Example 1: Get all ExpressRoute authorizations
```
PS C:\>$Circuit = Get-AzureRmExpressRouteCircuit -Name "ContosoCircuit" -ResourceGroupName "ContosoResourceGroup"
PS C:\> Get-AzureRmExpressRouteCircuitAuthorization -Circuit $Circuit
```

These commands return information about all the ExpressRoute authorizations associated with an ExpressRoute circuit.
The first command uses the **Get-AzureRmExpressRouteCircuit** cmdlet to create an object reference a circuit named ContosoCircuit; that object reference is stored in the variable $Circuit.
The second command then uses that object reference and the **Get-AzureRmExpressRouteCircuitAuthorization** cmdlet to return information about the authorizations associated with ContosoCircuit.

### Example 2: Get all ExpressRoute authorizations using the Where-Object cmdlet
```
PS C:\>$Circuit = Get-AzureRmExpressRouteCircuit -Name "ContosoCircuit" -ResourceGroupName "ContosoResourceGroup"
PS C:\> Get-AzureRmExpressRouteCircuitAuthorization -Circuit $Circuit | Where-Object {$_.AuthorizationUseStatus -eq "Available"}
```

These commands represent a variation on the commands used in Example 1.
In this case, however, information is returned only for those authorizations that are available for use (that is, for authorizations that have not been assigned to a virtual network).
To do this, the circuit authorization information is returned in command 2 and is piped to the **Where-Object** cmdlet.
**Where-Object** then picks out only those authorizations where the *AuthorizationUseStatus* property is set to Available.
To list only those authorizations that are not available, use this syntax for the Where clause:

{$_.AuthorizationUseStatus -ne "Available"}

## PARAMETERS

### -Name
Specifies the name of the ExpressRoute circuit authorization that this cmdlet gets.

-Name "ContosoCircuitAuthorization"

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

### -ExpressRouteCircuit
Specifies the ExpressRoute circuit authorization.

```yaml
Type: PSExpressRouteCircuit
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
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
@{Text=}```yaml
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

###  
**Get-AzureRmExpressRouteCircuitAuthorization** accepts pipelined instances of the **Microsoft.Azure.Commands.Network.Models.PSExpressRouteCircuit** object.

## OUTPUTS

###  
**Get-AzureRmExpressRouteCircuitAuthorization** returns instances of the **Microsoft.Azure.Commands.Network.Models.PSExpressRouteCircuitAuthorization** object.

## NOTES

## RELATED LINKS

[Add-AzureRmExpressRouteCircuitAuthorization](.\Add-AzureRmExpressRouteCircuitAuthorization.md)

[Get-AzureRmExpressRouteCircuit](.\Get-AzureRmExpressRouteCircuit.md)

[New-AzureRmExpressRouteCircuitAuthorization](.\New-AzureRmExpressRouteCircuitAuthorization.md)

[Remove-AzureRmExpressRouteCircuitAuthorization](.\Remove-AzureRmExpressRouteCircuitAuthorization.md)

