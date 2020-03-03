---
title: "userTeamwork resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userTeamwork resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userTeamworks](../api/userteamwork-list.md)|[userTeamwork](../resources/userTeamwork.md) collection|List properties and relationships of the [userTeamwork](../resources/userteamwork.md) objects.|
|[Get userTeamwork](../api/userteamwork-get.md)|[userTeamwork](../resources/userTeamwork.md)|Read properties and relationships of the [userTeamwork](../resources/userteamwork.md) object.|
|[Create userTeamwork](../api/userteamwork-create.md)|[userTeamwork](../resources/userTeamwork.md)|Create a new [userTeamwork](../resources/userteamwork.md) object.|
|[Delete userTeamwork](../api/userteamwork-delete.md)|None|Deletes a [userTeamwork](../resources/userteamwork.md).|
|[Update userTeamwork](../api/userteamwork-update.md)|[userTeamwork](../resources/userTeamwork.md)|Update the properties of a [userTeamwork](../resources/userteamwork.md) object.|
|[List installedApps](../api/userteamwork-list-installedapps.md)|[teamsAppInstallation](../resources/teamsAppInstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/userteamwork-post-installedapps.md)|[teamsAppInstallation](../resources/teamsAppInstallation.md)|Add installedApps by posting to the installedApps collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsAppInstallation.md) collection||

## JSON Representation
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

