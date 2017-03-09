---
external help file: Microsoft.Azure.Commands.EventHub.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureRmEventHub

## SYNOPSIS
Gets the details of a single Event Hub, or gets a list of Event Hubs.

## SYNTAX

```
Get-AzureRmEventHub [-ResourceGroupName] <String> [-NamespaceName] <String> [[-EventHubName] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmEventHub** cmdlet returns either the details of an Event Hub, or a list of all Event Hubs in the current namespace. If the Event Hub name is provided, the details of a single Event Hub are returned. If an Event Hub name is not provided, a list of all Event Hubs in the specified namespace is returned.

## EXAMPLES

### Example 1: Get details of an Event Hub
```
PS C:\> Get-AzureRmEventHub -ResourceGroupName "MyResourceGroupName" -NamespaceName "MyNamespaceName" -EventHubName "MyEventHubName"
```

This command gets the details of the Event Hub EventHubName.

### Example 2: Get a list of Event Hubs
```
PS C:\> Get-AzureRmEventHub -ResourceGroup "MyResourceGroupName" -NamespaceName "MyNamespaceName"
```

This command gets a list of Event Hubs in the namespace MyNamespaceName.

## PARAMETERS

### -EventHubName
Specifies the name of the Event Hub.

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

### -NamespaceName
Specifies the name of the Event Hubs namespace.

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

### -ResourceGroupName
Specifies the name of the resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.List`1[[Microsoft.Azure.Commands.EventHub.Models.EventHubAttributes, Microsoft.Azure.Commands.EventHub, Version=0.0.1.0, Culture=neutral, PublicKeyToken=null]]

## NOTES

## RELATED LINKS

[New-AzureRmEventHub](./New-AzureRmEventHub.md)

[Remove-AzureRmEventHub](./Remove-AzureRmEventHub.md)

[Set-AzureRmEventHub](./Set-AzureRmEventHub.md)