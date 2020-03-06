---
title: "userTeamwork resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userTeamwork resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userTeamwork](../api/userteamwork-get.md)|[userTeamwork](../resources/userteamwork.md)|Read properties and relationships of the [userTeamwork](../resources/userteamwork.md) object.|
|[Update userTeamwork](../api/userteamwork-update.md)|[userTeamwork](../resources/userteamwork.md)|Update the properties of a [userTeamwork](../resources/userteamwork.md) object.|
|[List installedApps](../api/userteamwork-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/userteamwork-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Add installedApps by posting to the installedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userTeamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTeamwork",
  "id": "String (identifier)"
}
```

