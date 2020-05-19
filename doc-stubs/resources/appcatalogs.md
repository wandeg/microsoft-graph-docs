---
title: "appCatalogs resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appCatalogs resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teamsApps](../api/appcatalogs-list-teamsapps.md)|[teamsApp](../resources/teamsapp.md) collection|Get the teamsApps from the teamsApps navigation property.|
|[Create teamsApps](../api/appcatalogs-post-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Create a new teamsApps object.|
|[Delete teamsApps](../api/appcatalogs-delete-teamsapps.md)|None|Delete a [teamsApp](../resources/teamsapp.md) object.|
|[Update teamsApps](../api/appcatalogs-update-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Update the properties of a teamsApps object.|
|[Get teamsApps](../api/appcatalogs-get-teamsapp.md)|[teamsApp](../resources/teamsapp.md)|Read the properties and relationships of a [teamsApp](../resources/teamsapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApps|[teamsApp](../resources/teamsapp.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appCatalogs",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appCatalogs",
  "id": "String (identifier)"
}
```

