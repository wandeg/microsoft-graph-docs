---
title: "privilegedRoleSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# privilegedRoleSettings resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedRoleSettingses](../api/privilegedrolesettings-list.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md) collection|List properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) objects.|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)|Read properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Create privilegedRoleSettings](../api/privilegedrolesettings-create.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)|Create a new [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Delete privilegedRoleSettings](../api/privilegedrolesettings-delete.md)|None|Deletes a [privilegedRoleSettings](../resources/privilegedrolesettings.md).|
|[Update privilegedRoleSettings](../api/privilegedrolesettings-update.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)|Update the properties of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|approvalOnElevation|Boolean||
|approverIds|String collection||
|elevationDuration|Duration||
|id|String| Inherited from [entity](../resources/entity.md)|
|isMfaOnElevationConfigurable|Boolean||
|lastGlobalAdmin|Boolean||
|maxElavationDuration|Duration||
|mfaOnElevation|Boolean||
|minElevationDuration|Duration||
|notificationToUserOnElevation|Boolean||
|ticketingInfoOnElevation|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "mfaOnElevation": true,
  "lastGlobalAdmin": true,
  "isMfaOnElevationConfigurable": true,
  "approvalOnElevation": true
}
```

