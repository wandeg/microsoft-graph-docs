---
title: "invitation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# invitation resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List invitations](../api/invitation-list.md)|[invitation](../resources/invitation.md) collection|Get a list of the [invitation](../resources/invitation.md) objects and their properties.|
|[Get invitation](../api/invitation-get.md)|[invitation](../resources/invitation.md)|Read properties and relationships of an [invitation](../resources/invitation.md) object.|
|[Create invitation](../api/invitation-post-invitations.md)|[invitation](../resources/invitation.md)|Create a new [invitation](../resources/invitation.md) object.|
|[Delete invitation](../api/invitation-delete.md)|None|Deletes an [invitation](../resources/invitation.md).|
|[Update invitation](../api/invitation-update.md)|[invitation](../resources/invitation.md)|Update the properties of a [invitation](../resources/invitation.md) object.|
|[List invitedUser](../api/invitation-list-inviteduser.md)|[user](../resources/user.md) collection|Get the users from the invitedUser navigation property.|
|[Add invitedUser](../api/invitation-post-inviteduser.md)|[user](../resources/user.md)|Add invitedUser by posting to the invitedUser collection.|
|[Remove invitedUser](../api/invitation-delete-inviteduser.md)|None|Remove an invitedUser object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invitedUserDisplayName|String|**TODO: Add Description**|
|invitedUserEmailAddress|String|**TODO: Add Description**|
|invitedUserMessageInfo|[invitedUserMessageInfo](../resources/invitedusermessageinfo.md)|**TODO: Add Description**|
|invitedUserType|String|**TODO: Add Description**|
|inviteRedeemUrl|String|**TODO: Add Description**|
|inviteRedirectUrl|String|**TODO: Add Description**|
|sendInvitationMessage|Boolean|**TODO: Add Description**|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|invitedUser|[user](../resources/user.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invitation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.invitation",
  "id": "String (identifier)",
  "invitedUserDisplayName": "String",
  "invitedUserType": "String",
  "invitedUserEmailAddress": "String",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "address": "String"
        }
      }
    ],
    "messageLanguage": "String",
    "customizedMessageBody": "String"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "String",
  "inviteRedeemUrl": "String",
  "status": "String"
}
```

