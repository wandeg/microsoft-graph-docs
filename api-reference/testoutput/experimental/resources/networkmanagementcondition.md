---
title: "networkManagementCondition resource type"
description: "Contains the information to define a network management condition."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# networkManagementCondition resource type


Namespace: microsoft.graph

Contains the information to define a network management condition.


Inherits from [managementCondition](../resources/managementcondition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List networkManagementConditions](../api/networkmanagementcondition-list.md)|[networkManagementCondition](../resources/networkmanagementcondition.md) collection|List properties and relationships of the [networkManagementCondition](../resources/networkmanagementcondition.md) objects.|
|[Get networkManagementCondition](../api/networkmanagementcondition-get.md)|[networkManagementCondition](../resources/networkmanagementcondition.md)|Read properties and relationships of the [networkManagementCondition](../resources/networkmanagementcondition.md) object.|
|[List managementConditionStatements](../api/networkmanagementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/networkmanagementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementcondition.md)|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementcondition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
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
  "@odata.type": "microsoft.graph.networkManagementCondition",
  "baseType": "microsoft.graph.managementCondition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```

