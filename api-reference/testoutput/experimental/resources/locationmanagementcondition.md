---
title: "locationManagementCondition resource type"
description: "Contains the information to define a location management condition, an area of interest, to monitor."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# locationManagementCondition resource type

Contains the information to define a location management condition, an area of interest, to monitor.


Inherits from [managementCondition](../resources/managementCondition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List locationManagementConditions](../api/locationmanagementcondition-list.md)|[locationManagementCondition](../resources/locationManagementCondition.md) collection|List properties and relationships of the [locationManagementCondition](../resources/locationmanagementcondition.md) objects.|
|[Get locationManagementCondition](../api/locationmanagementcondition-get.md)|[locationManagementCondition](../resources/locationManagementCondition.md)|Read properties and relationships of the [locationManagementCondition](../resources/locationmanagementcondition.md) object.|
|[List managementConditionStatements](../api/locationmanagementcondition-list-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md) collection|Get the managementConditionStatements from the managementConditionStatements navigation property.|
|[Create managementConditionStatements](../api/locationmanagementcondition-post-managementconditionstatements.md)|[managementConditionStatement](../resources/managementConditionStatement.md)|Create managementConditionStatements by posting to the managementConditionStatements collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
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
  "@odata.type": "microsoft.graph.locationManagementCondition",
  "baseType": "microsoft.graph.managementCondition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
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

