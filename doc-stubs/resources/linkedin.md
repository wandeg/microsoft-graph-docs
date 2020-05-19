---
title: "linkedIn resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# linkedIn resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List invitations](../api/linkedin-list-invitations.md)|[InvitationV2](../resources/invitationv2.md) collection|Get the InvitationV2 from the invitations navigation property.|
|[Create invitations](../api/linkedin-post-invitations.md)|[InvitationV2](../resources/invitationv2.md)|Create a new invitations object.|
|[Delete invitations](../api/linkedin-delete-invitations.md)|None|Delete an [InvitationV2](../resources/invitationv2.md) object.|
|[Update invitations](../api/linkedin-update-invitations.md)|[InvitationV2](../resources/invitationv2.md)|Update the properties of an invitations object.|
|[Get invitations](../api/linkedin-get-invitationv2.md)|[InvitationV2](../resources/invitationv2.md)|Read the properties and relationships of an [InvitationV2](../resources/invitationv2.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|invitations|[InvitationV2](../resources/invitationv2.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedIn",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedIn",
  "id": "String (identifier)"
}
```

