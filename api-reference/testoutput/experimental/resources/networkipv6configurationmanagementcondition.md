---
title: "networkIPv6ConfigurationManagementCondition resource type"
description: "IPv6 configuration-based management conditions may be defined that will trigger when a device detects certain IP network settings. An IP config management condition will only be considered TRUE when the network connection is active.
IPv6 DHCP server addresses may not be matched. This is because Windows(circa Redstone) does not expose this information to the Natural Authentication service."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# networkIPv6ConfigurationManagementCondition resource type

IPv6 configuration-based management conditions may be defined that will trigger when a device detects certain IP network settings. An IP config management condition will only be considered TRUE when the network connection is active.
IPv6 DHCP server addresses may not be matched. This is because Windows(circa Redstone) does not expose this information to the Natural Authentication service.


Inherits from [networkManagementCondition](../resources/networkManagementCondition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List networkIPv6ConfigurationManagementConditions](../api/networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/networkIPv6ConfigurationManagementCondition.md) collection|List properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) objects.|
|[Get networkIPv6ConfigurationManagementCondition](../api/networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/networkIPv6ConfigurationManagementCondition.md)|Read properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object.|
|[Create networkIPv6ConfigurationManagementCondition](../api/networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/networkIPv6ConfigurationManagementCondition.md)|Create a new [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object.|
|[Delete networkIPv6ConfigurationManagementCondition](../api/networkipv6configurationmanagementcondition-delete.md)|None|Deletes a [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md).|
|[Update networkIPv6ConfigurationManagementCondition](../api/networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/networkIPv6ConfigurationManagementCondition.md)|Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/networkipv6configurationmanagementcondition.md) object.|
|[List managementConditionStatements](../api/networkipv6configurationmanagementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/networkipv6configurationmanagementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|dnsSuffixList|String collection|Valid DNS suffixes for the current network. e.g. seattle.contoso.com|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipV6DNSServerList|String collection|An IPv6 DNS servers configured for the adapter.|
|ipV6Gateway|String|The IPv6 gateway address to. e.g 2001:db8::1|
|ipV6Prefix|String|The IPv6 subnet to be connected to. e.g. 2001:db8::/32|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions. Inherited from [managementCondition](../resources/managementCondition.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/managementConditionStatement.md) collection|The management condition statements associated to the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "baseType": "microsoft.graph.networkManagementCondition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
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
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```

