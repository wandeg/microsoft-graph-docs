---
title: "linkedIn resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# linkedIn resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get linkedIn](../api/linkedin-get.md)|[linkedIn](../resources/linkedin.md)|Read properties and relationships of the [linkedIn](../resources/linkedin.md) object.|
|[Update linkedIn](../api/linkedin-update.md)|[linkedIn](../resources/linkedin.md)|Update the properties of a [linkedIn](../resources/linkedin.md) object.|
|[List invitations](../api/linkedin-list-invitations.md)|[InvitationV2](../resources/invitationv2.md) collection|Get the InvitationV2s from the invitations navigation property.|
|[Add invitations](../api/linkedin-post-invitations.md)|[InvitationV2](../resources/invitationv2.md)|Add invitations by posting to the invitations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|invitations|[InvitationV2](../resources/invitationv2.md) collection||

## JSON representation
Here is a JSON representation of the resource.
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

