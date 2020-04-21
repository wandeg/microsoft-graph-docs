---
title: "appCatalogs resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# appCatalogs resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appCatalogs](../api/appcatalogs-get.md)|[appCatalogs](../resources/appcatalogs.md)|Read properties and relationships of an [appCatalogs](../resources/appcatalogs.md) object.|
|[Update appCatalogs](../api/appcatalogs-update.md)|[appCatalogs](../resources/appcatalogs.md)|Update the properties of a [appCatalogs](../resources/appcatalogs.md) object.|
|[List teamsApps](../api/appcatalogs-list-teamsapps.md)|[teamsApp](../resources/teamsapp.md) collection|Get the teamsApps from the teamsApps navigation property.|
|[Create teamsApps](../api/appcatalogs-post-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Create a new teamsApps object.|
|[Delete teamsApps](../api/appcatalogs-delete-teamsapps.md)|None|Delete a teamsApps object.|
|[Update teamsApps](../api/appcatalogs-update-teamsapps.md)|[teamsApp](../resources/teamsapp.md)|Update the properties of a teamsApps object.|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsapp.md)|Read properties and relationships of a [teamsApp](../resources/teamsapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApps|[teamsApp](../resources/teamsapp.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
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

