---
title: "user resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# user resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List profile](../api/user-list-profile.md)|[profile](../resources/profile.md) collection|Get the profiles from the profile navigation property.|
|[Create profile](../api/user-post-profile.md)|[profile](../resources/profile.md)|Create a new profile object.|
|[Delete profile](../api/user-delete-profile.md)|None|Delete a [profile](../resources/profile.md) object.|
|[Update profile](../api/user-update-profile.md)|[profile](../resources/profile.md)|Update the properties of a profile object.|
|[Get profile](../api/user-get-profile.md)|[profile](../resources/profile.md)|Read the properties and relationships of a [profile](../resources/profile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|profile|[profile](../resources/profile.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```

