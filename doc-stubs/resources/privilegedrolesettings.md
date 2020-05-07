---
title: "privilegedRoleSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedRoleSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalOnElevation|Boolean|**TODO: Add Description**|
|approverIds|String collection|**TODO: Add Description**|
|elevationDuration|Duration|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isMfaOnElevationConfigurable|Boolean|**TODO: Add Description**|
|lastGlobalAdmin|Boolean|**TODO: Add Description**|
|maxElavationDuration|Duration|**TODO: Add Description**|
|mfaOnElevation|Boolean|**TODO: Add Description**|
|minElevationDuration|Duration|**TODO: Add Description**|
|notificationToUserOnElevation|Boolean|**TODO: Add Description**|
|ticketingInfoOnElevation|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedRoleSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedRoleSettings",
  "id": "String (identifier)",
  "approverIds": [
    "String"
  ],
  "minElevationDuration": "String (duration)",
  "maxElavationDuration": "String (duration)",
  "elevationDuration": "String (duration)",
  "notificationToUserOnElevation": "Boolean",
  "ticketingInfoOnElevation": "Boolean",
  "mfaOnElevation": "Boolean",
  "lastGlobalAdmin": "Boolean",
  "isMfaOnElevationConfigurable": "Boolean",
  "approvalOnElevation": "Boolean"
}
```

