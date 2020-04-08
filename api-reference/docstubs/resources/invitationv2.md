---
title: "InvitationV2 resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# InvitationV2 resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get InvitationV2](../api/invitationv2-get.md)|[InvitationV2](../resources/invitationv2.md)|Read properties and relationships of the [InvitationV2](../resources/invitationv2.md) object.|
|[Update InvitationV2](../api/invitationv2-update.md)|[InvitationV2](../resources/invitationv2.md)|Update the properties of a [InvitationV2](../resources/invitationv2.md) object.|
|[inviteeClosingInvitation](../api/invitationv2-inviteeclosinginvitation.md)|[InviteActionResults](../resources/inviteactionresults.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|created|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|invitee|String||
|inviter|String||
|lastModified|Int64||
|message|[InvitationV2Message](../resources/invitationv2message.md)||
|trackingId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.InvitationV2",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.InvitationV2",
  "id": "String (identifier)",
  "created": 1024,
  "lastModified": 1024,
  "inviter": "String",
  "invitee": "String",
  "message": {
    "@odata.type": "microsoft.graph.InvitationV2Message"
  },
  "trackingId": "String"
}
```

