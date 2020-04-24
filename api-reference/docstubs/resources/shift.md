---
title: "shift resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# shift resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get shift](../api/shift-get.md)|[shift](../resources/shift.md)|Read the properties and relationships of a [shift](../resources/shift.md) object.|
|[Update shift](../api/shift-update.md)|[shift](../resources/shift.md)|Update the properties of a [shift](../resources/shift.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|draftShift|[shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|schedulingGroupId|String|**TODO: Add Description**|
|sharedShift|[shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

