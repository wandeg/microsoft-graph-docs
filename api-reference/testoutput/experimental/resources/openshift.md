---
title: "openShift resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# openShift resource type


Namespace: microsoft.graph




Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List openShifts](../api/openshift-list.md)|[openShift](../resources/openshift.md) collection|List properties and relationships of the [openShift](../resources/openshift.md) objects.|
|[Get openShift](../api/openshift-get.md)|[openShift](../resources/openshift.md)|Read properties and relationships of the [openShift](../resources/openshift.md) object.|
|[Create openShift](../api/openshift-create.md)|[openShift](../resources/openshift.md)|Create a new [openShift](../resources/openshift.md) object.|
|[Delete openShift](../api/openshift-delete.md)|None|Deletes a [openShift](../resources/openshift.md).|
|[Update openShift](../api/openshift-update.md)|[openShift](../resources/openshift.md)|Update the properties of a [openShift](../resources/openshift.md) object.|
|[List openShifts](../api/schedule-list-openshifts.md)|[openShift](../resources/openshift.md) collection|Get the openShifts from the openShifts navigation property.|
|[Add openShifts](../api/schedule-post-openshifts.md)|[openShift](../resources/openshift.md)|Add openShifts by posting to the openShifts collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|draftOpenShift|[openShiftItem](../resources/openshiftitem.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|schedulingGroupId|String||
|sharedOpenShift|[openShiftItem](../resources/openshiftitem.md)||

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

