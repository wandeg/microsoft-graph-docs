---
title: "invitation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# invitation resource type


Namespace: Microsoft.AADInviteMgr

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List invitations](../api/microsoft.aadinvitemgr-invitation-list.md)|[invitation](../resources/microsoft.aadinvitemgr-invitation.md) collection|Get a list of the [invitation](../resources/invitation.md) objects and their properties.|
|[Get invitation](../api/microsoft.aadinvitemgr-invitation-get.md)|[invitation](../resources/microsoft.aadinvitemgr-invitation.md)|Read properties and relationships of an [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object.|
|[Create invitation](../api/microsoft.aadinvitemgr-invitation-post-invitations.md)|[invitation](../resources/microsoft.aadinvitemgr-invitation.md)|Create a new [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object.|
|[Delete invitation](../api/microsoft.aadinvitemgr-invitation-delete.md)|None|Deletes an [invitation](../resources/microsoft.aadinvitemgr-invitation.md).|
|[Update invitation](../api/microsoft.aadinvitemgr-invitation-update.md)|[invitation](../resources/microsoft.aadinvitemgr-invitation.md)|Update the properties of a [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object.|
|[List invitedUser](../api/microsoft.aadinvitemgr-invitation-list-inviteduser.md)|[user](../resources/microsoft.aadinvitemgr-user.md) collection|Get the users from the invitedUser navigation property.|
|[Add invitedUser](../api/microsoft.aadinvitemgr-invitation-post-inviteduser.md)|[user](../resources/microsoft.aadinvitemgr-user.md)|Add invitedUser by posting to the invitedUser collection.|
|[Remove invitedUser](../api/microsoft.aadinvitemgr-invitation-delete-inviteduser.md)|None|Remove an invitedUser object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|invitedUserDisplayName|String|**TODO: Add Description**|
|invitedUserEmailAddress|String|**TODO: Add Description**|
|InvitedUserMessageInfo|[invitedUserMessageInfo](../resources/microsoft.aadinvitemgr-invitedusermessageinfo.md)|**TODO: Add Description**|
|invitedUserType|String|**TODO: Add Description**|
|inviteRedeemUrl|String|**TODO: Add Description**|
|inviteRedirectUrl|String|**TODO: Add Description**|
|resetRedemption|Boolean|**TODO: Add Description**|
|sendInvitationMessage|Boolean|**TODO: Add Description**|
|status|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|invitedUser|[user](../resources/microsoft.aadinvitemgr-user.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AADInviteMgr.invitation",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AADInviteMgr.invitation",
  "id": "String (identifier)",
  "invitedUserDisplayName": "String",
  "invitedUserType": "String",
  "invitedUserEmailAddress": "String",
  "InvitedUserMessageInfo": {
    "@odata.type": "Microsoft.AADInviteMgr.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "Microsoft.AADInviteMgr.recipient",
        "emailAddress": {
          "@odata.type": "Microsoft.AADInviteMgr.emailAddress",
          "name": "String",
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
  "status": "String",
  "resetRedemption": true
}
```

