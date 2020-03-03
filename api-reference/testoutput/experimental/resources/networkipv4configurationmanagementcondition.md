---
title: "networkIPv4ConfigurationManagementCondition resource type"
description: "IPv4 configuration-based management conditions may be defined that will trigger when a device detects certain IP network settings. An IP config management conditions will only be considered TRUE when the network connection is active."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# networkIPv4ConfigurationManagementCondition resource type


Namespace: microsoft.graph

IPv4 configuration-based management conditions may be defined that will trigger when a device detects certain IP network settings. An IP config management conditions will only be considered TRUE when the network connection is active.


Inherits from [networkManagementCondition](../resources/networkmanagementcondition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List networkIPv4ConfigurationManagementConditions](../api/networkipv4configurationmanagementcondition-list.md)|[networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) collection|List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) objects.|
|[Get networkIPv4ConfigurationManagementCondition](../api/networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md)|Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) object.|
|[Create networkIPv4ConfigurationManagementCondition](../api/networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md)|Create a new [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) object.|
|[Delete networkIPv4ConfigurationManagementCondition](../api/networkipv4configurationmanagementcondition-delete.md)|None|Deletes a [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md).|
|[Update networkIPv4ConfigurationManagementCondition](../api/networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md)|Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) object.|
|[List managementConditionStatements](../api/networkipv4configurationmanagementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/networkipv4configurationmanagementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|dnsSuffixList|String collection|Valid DNS suffixes for the current network. e.g. seattle.contoso.com|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipV4DHCPServer|String|The IPv4 address of the DHCP server for the adapter.|
|ipV4DNSServerList|String collection|The IPv4 DNS servers configured for the adapter.|
|ipV4Gateway|String|The IPv4 gateway address. e.g. 10.0.0.0|
|ipV4Prefix|String|The IPv4 subnet to be connected to. e.g. 10.0.0.0/8|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions. Inherited from [managementCondition](../resources/managementcondition.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/managementconditionstatement.md) collection|The management condition statements associated to the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "baseType": "microsoft.graph.networkManagementCondition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```

