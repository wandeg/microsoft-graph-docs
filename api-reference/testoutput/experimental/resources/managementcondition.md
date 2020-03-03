---
title: "managementCondition resource type"
description: "Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managementCondition resource type


Namespace: microsoft.graph

Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List managementConditions](../api/managementcondition-list.md)|[managementCondition](../resources/managementcondition.md) collection|List properties and relationships of the [managementCondition](../resources/managementcondition.md) objects.|
|[Get managementCondition](../api/managementcondition-get.md)|[managementCondition](../resources/managementcondition.md)|Read properties and relationships of the [managementCondition](../resources/managementcondition.md) object.|
|[getManagementConditionsForPlatform](../api/managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/managementcondition.md) collection||
|[List managementConditionStatements](../api/managementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/managementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition.|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side.|
|description|String|The admin defined description of the management condition.|
|displayName|String|The admin defined name of the management condition.|
|eTag|String|ETag of the management condition. Updated service side.|
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side.|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/managementconditionstatement.md) collection|The management condition statements associated to the management condition.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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

