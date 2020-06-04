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

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List defaultRolesSettings](../api/tenantsetupinfo-list-defaultrolessettings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md) collection|Get the privilegedRoleSettings from the defaultRolesSettings navigation property.|
|[Add defaultRolesSettings](../api/tenantsetupinfo-post-defaultrolessettings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Add defaultRolesSettings by posting to the defaultRolesSettings collection.|
|[Remove defaultRolesSettings](../api/tenantsetupinfo-delete-defaultrolessettings.md)|None|Remove a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[List privilegedRoleSettings](../api/privilegedrolesettings-list.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md) collection|Get a list of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) objects and their properties.|
|[Create privilegedRoleSettings](../api/privilegedrolesettings-create.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Create a new [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Read the properties and relationships of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Update privilegedRoleSettings](../api/privilegedrolesettings-update.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Update the properties of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|
|[Delete privilegedRoleSettings](../api/privilegedrolesettings-delete.md)|None|Deletes a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|

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

