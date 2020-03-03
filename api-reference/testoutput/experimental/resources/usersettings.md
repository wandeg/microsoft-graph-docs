---
title: "userSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userSettings resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userSettingses](../api/usersettings-list.md)|[userSettings](../resources/usersettings.md) collection|List properties and relationships of the [userSettings](../resources/usersettings.md) objects.|
|[Get userSettings](../api/usersettings-get.md)|[userSettings](../resources/usersettings.md)|Read properties and relationships of the [userSettings](../resources/usersettings.md) object.|
|[Create userSettings](../api/usersettings-create.md)|[userSettings](../resources/usersettings.md)|Create a new [userSettings](../resources/usersettings.md) object.|
|[Delete userSettings](../api/usersettings-delete.md)|None|Deletes a [userSettings](../resources/usersettings.md).|
|[Update userSettings](../api/usersettings-update.md)|[userSettings](../resources/usersettings.md)|Update the properties of a [userSettings](../resources/usersettings.md) object.|
|[Get shiftPreferences](../api/shiftpreferences-get.md)|[shiftPreferences](../resources/shiftpreferences.md)|Read properties and relationships of the [shiftPreferences](../resources/shiftpreferences.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean||
|contributionToContentDiscoveryDisabled|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|shiftPreferences|[shiftPreferences](../resources/shiftpreferences.md)||

## JSON Representation
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

