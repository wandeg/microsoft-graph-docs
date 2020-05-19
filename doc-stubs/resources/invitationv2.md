---
title: "InvitationV2 resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# InvitationV2 resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[inviteeClosingInvitation](../api/invitationv2-inviteeclosinginvitation.md)|[InviteActionResults](../resources/inviteactionresults.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|created|Int64|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invitee|String|**TODO: Add Description**|
|inviter|String|**TODO: Add Description**|
|lastModified|Int64|**TODO: Add Description**|
|message|[InvitationV2Message](../resources/invitationv2message.md)|**TODO: Add Description**|
|trackingId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "created": "Integer",
  "lastModified": "Integer",
  "inviter": "String",
  "invitee": "String",
  "message": {
    "@odata.type": "microsoft.graph.InvitationV2Message"
  },
  "trackingId": "String"
}
```

