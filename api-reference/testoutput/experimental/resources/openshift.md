---
title: "openShift resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# openShift resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get openShift](../api/openshift-get.md)|[openShift](../resources/openShift.md)|Read properties and relationships of the [openShift](../resources/openshift.md) object.|
|[Delete openShift](../api/openshift-delete.md)|None|Deletes a [openShift](../resources/openshift.md).|
|[Update openShift](../api/openshift-update.md)|[openShift](../resources/openShift.md)|Update the properties of a [openShift](../resources/openshift.md) object.|
|[List openShifts](../api/schedule-list-openshifts.md)|[openShift](../resources/openShift.md) collection|Get the openShifts from the openShifts navigation property.|
|[Add openShifts](../api/schedule-post-openshifts.md)|[openShift](../resources/openShift.md)|Add openShifts by posting to the openShifts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|draftOpenShift|[openShiftItem](../resources/openShiftItem.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|schedulingGroupId|String||
|sharedOpenShift|[openShiftItem](../resources/openShiftItem.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.openShift",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.openShift",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedOpenShift": {
    "@odata.type": "microsoft.graph.openShiftItem"
  },
  "draftOpenShift": {
    "@odata.type": "microsoft.graph.openShiftItem"
  },
  "schedulingGroupId": "String"
}
```

