---
title: "managementCondition resource type"
description: "Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managementCondition resource type


Namespace: microsoft.graph

Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managementCondition](../api/managementcondition-get.md)|[managementCondition](../resources/managementcondition.md)|Read the properties and relationships of a [managementCondition](../resources/managementcondition.md) object.|
|[getManagementConditionsForPlatform](../api/managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/managementcondition.md) collection|**TODO: Add Description**|
|[List managementConditionStatements](../api/managementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Add managementConditionStatements](../api/managementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementconditionstatement.md)|Add managementConditionStatements by posting to the managementConditionStatements collection.|
|[Remove managementConditionStatements](../api/managementcondition-delete-managementconditionstatements.md)|None|Remove a [managementConditionStatement](../resources/managementconditionstatement.md) object.|
|[List managementConditions](../api/managementconditionstatement-list-managementconditions.md)|[managementCondition](../resources/managementcondition.md) collection|Get the managementConditions from the managementConditions navigation property.|
|[Add managementConditions](../api/managementconditionstatement-post-managementconditions.md)|[managementCondition](../resources/managementcondition.md)|Add managementConditions by posting to the managementConditions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|devicePlatformType collection|The applicable platforms for this management condition.|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side.|
|description|String|The admin defined description of the management condition.|
|displayName|String|The admin defined name of the management condition.|
|eTag|String|ETag of the management condition. Updated service side.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side.|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/managementconditionstatement.md) collection|The management condition statements associated to the management condition.|

## JSON representation
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

