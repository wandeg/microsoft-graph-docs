---
title: "teamsTab resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsTab resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teamsApp](../api/teamstab-list-teamsapp.md)|[teamsApp](../resources/teamsapp.md) collection|Get the teamsApps from the teamsApp navigation property.|
|[Add teamsApp](../api/teamstab-post-teamsapp.md)|[teamsApp](../resources/teamsapp.md)|Add teamsApp by posting to the teamsApp collection.|
|[Remove teamsApp](../api/teamstab-delete-teamsapp.md)|None|Remove a [teamsApp](../resources/teamsapp.md) object.|
|[List tabs](../api/channel-list-tabs.md)|[teamsTab](../resources/teamstab.md) collection|Get the teamsTabs from the tabs navigation property.|
|[Create tabs](../api/channel-post-tabs.md)|[teamsTab](../resources/teamstab.md)|Create a new tabs object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|[teamsTabConfiguration](../resources/teamstabconfiguration.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|messageId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|sortOrderIndex|String|**TODO: Add Description**|
|teamsAppId|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApp|[teamsApp](../resources/teamsapp.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsTab",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsTab",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "teamsAppId": "String",
  "sortOrderIndex": "String",
  "messageId": "String",
  "webUrl": "String",
  "configuration": {
    "@odata.type": "microsoft.graph.teamsTabConfiguration"
  }
}
```

