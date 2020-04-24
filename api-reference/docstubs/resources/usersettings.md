---
title: "userSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/usersettings.md)|Read the properties and relationships of a [userSettings](../resources/usersettings.md) object.|
|[Update userSettings](../api/usersettings-update.md)|[userSettings](../resources/usersettings.md)|Update the properties of a [userSettings](../resources/usersettings.md) object.|
|[List shiftPreferences](../api/usersettings-list-shiftpreferences.md)|[shiftPreferences](../resources/shiftpreferences.md) collection|Get the shiftPreferences from the shiftPreferences navigation property.|
|[Create shiftPreferences](../api/usersettings-post-shiftpreferences.md)|[shiftPreferences](../resources/shiftpreferences.md)|Create a new shiftPreferences object.|
|[Delete shiftPreferences](../api/usersettings-delete-shiftpreferences.md)|None|Delete a [shiftPreferences](../resources/shiftpreferences.md) object.|
|[Update shiftPreferences](../api/usersettings-update-shiftpreferences.md)|[shiftPreferences](../resources/shiftpreferences.md)|Update the properties of a shiftPreferences object.|
|[Get shiftPreferences](../api/shiftpreferences-get.md)|[shiftPreferences](../resources/shiftpreferences.md)|Read the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean|**TODO: Add Description**|
|contributionToContentDiscoveryDisabled|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|shiftPreferences|[shiftPreferences](../resources/shiftpreferences.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "String (identifier)",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

