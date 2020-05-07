---
title: "DecoratedProfileConnection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# DecoratedProfileConnection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List DecoratedProfileConnections](../api/decoratedprofileconnection-list.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md) collection|Get a list of the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) objects and their properties.|
|[Get DecoratedProfileConnection](../api/decoratedprofileconnection-get.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Read the properties and relationships of a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[Create DecoratedProfileConnection](../api/decoratedprofileconnection-post-decoratedprofileconnections.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Create a new [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[Delete DecoratedProfileConnection](../api/decoratedprofileconnection-delete.md)|None|Deletes a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[Update DecoratedProfileConnection](../api/decoratedprofileconnection-update.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Update the properties of a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[viewer](../api/decoratedprofileconnection-viewer.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md) collection|**TODO: Add Description**|
|[List profile](../api/decoratedprofileconnection-list-profile.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get the DecoratedProfiles from the profile navigation property.|
|[Create profile](../api/decoratedprofileconnection-post-profile.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Create a new profile object.|
|[Delete profile](../api/decoratedprofileconnection-delete-profile.md)|None|Delete a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Update profile](../api/decoratedprofileconnection-update-profile.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Update the properties of a profile object.|
|[Get DecoratedProfile](../api/decoratedprofile-get.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Read the properties and relationships of a [DecoratedProfile](../resources/decoratedprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|relevanceScore|Double|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|profile|[DecoratedProfile](../resources/decoratedprofile.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.DecoratedProfileConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "id": "String (identifier)",
  "relevanceScore": "Double"
}
```

