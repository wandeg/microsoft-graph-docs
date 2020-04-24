---
title: "userTeamwork resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userTeamwork resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userTeamwork](../api/userteamwork-get.md)|[userTeamwork](../resources/userteamwork.md)|Read the properties and relationships of a [userTeamwork](../resources/userteamwork.md) object.|
|[Update userTeamwork](../api/userteamwork-update.md)|[userTeamwork](../resources/userteamwork.md)|Update the properties of a [userTeamwork](../resources/userteamwork.md) object.|
|[List installedApps](../api/userteamwork-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Create installedApps](../api/userteamwork-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Create a new installedApps object.|
|[Delete installedApps](../api/userteamwork-delete-installedapps.md)|None|Delete an [teamsAppInstallation](../resources/teamsappinstallation.md) object.|
|[Update installedApps](../api/userteamwork-update-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Update the properties of an installedApps object.|
|[Get teamsAppInstallation](../api/teamsappinstallation-get.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Read the properties and relationships of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|**TODO: Add Description**|

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

