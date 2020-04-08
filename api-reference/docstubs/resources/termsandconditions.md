---
title: "termsAndConditions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# termsAndConditions resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read properties and relationships of the [termsAndConditions](../resources/termsandconditions.md) object.|
|[Update termsAndConditions](../api/termsandconditions-update.md)|[termsAndConditions](../resources/termsandconditions.md)|Update the properties of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List groupAssignments](../api/termsandconditions-list-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignments from the groupAssignments navigation property.|
|[Add groupAssignments](../api/termsandconditions-post-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Add groupAssignments by posting to the groupAssignments collection.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignments from the assignments navigation property.|
|[Add assignments](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Add assignments by posting to the assignments collection.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatuses from the acceptanceStatuses navigation property.|
|[Add acceptanceStatuses](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Add acceptanceStatuses by posting to the acceptanceStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptanceStatement|String||
|bodyText|String||
|createdDateTime|DateTimeOffset||
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||
|title|String||
|version|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection||
|assignments|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection||
|groupAssignments|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```

