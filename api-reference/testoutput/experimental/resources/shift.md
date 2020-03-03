---
title: "shift resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# shift resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get shift](../api/shift-get.md)|[shift](../resources/shift.md)|Read properties and relationships of the [shift](../resources/shift.md) object.|
|[Delete shift](../api/shift-delete.md)|None|Deletes a [shift](../resources/shift.md).|
|[Update shift](../api/shift-update.md)|[shift](../resources/shift.md)|Update the properties of a [shift](../resources/shift.md) object.|
|[List shifts](../api/schedule-list-shifts.md)|[shift](../resources/shift.md) collection|Get the shifts from the shifts navigation property.|
|[Add shifts](../api/schedule-post-shifts.md)|[shift](../resources/shift.md)|Add shifts by posting to the shifts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|draftShift|[shiftItem](../resources/shiftItem.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|schedulingGroupId|String||
|sharedShift|[shiftItem](../resources/shiftItem.md)||
|userId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shift",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "String",
  "schedulingGroupId": "String"
}
```

