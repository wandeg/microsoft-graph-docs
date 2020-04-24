---
title: "openShift resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# openShift resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get openShift](../api/openshift-get.md)|[openShift](../resources/openshift.md)|Read the properties and relationships of an [openShift](../resources/openshift.md) object.|
|[Update openShift](../api/openshift-update.md)|[openShift](../resources/openshift.md)|Update the properties of an [openShift](../resources/openshift.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|draftOpenShift|[openShiftItem](../resources/openshiftitem.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|schedulingGroupId|String|**TODO: Add Description**|
|sharedOpenShift|[openShiftItem](../resources/openshiftitem.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

