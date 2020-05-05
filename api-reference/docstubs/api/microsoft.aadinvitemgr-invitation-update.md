---
title: "Update invitation"
description: "Update the properties of a invitation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update invitation

Namespace: Microsoft.AADInviteMgr

Update the properties of a [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /invitations/{invitationsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object.

The following table shows the properties that are required when you create the [invitation](../resources/microsoft.aadinvitemgr-invitation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|invitedUserDisplayName|String|**TODO: Add Description**|
|invitedUserType|String|**TODO: Add Description**|
|invitedUserEmailAddress|String|**TODO: Add Description**|
|InvitedUserMessageInfo|[invitedUserMessageInfo](../resources/microsoft.aadinvitemgr-invitedusermessageinfo.md)|**TODO: Add Description**|
|sendInvitationMessage|Boolean|**TODO: Add Description**|
|inviteRedirectUrl|String|**TODO: Add Description**|
|inviteRedeemUrl|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|resetRedemption|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [invitation](../resources/microsoft.aadinvitemgr-invitation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_invitation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}
Content-Type: application/json
Content-length: 958

{
  "@odata.type": "#Microsoft.AADInviteMgr.invitation",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "InvitedUserMessageInfo": {
    "@odata.type": "Microsoft.AADInviteMgr.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "Microsoft.AADInviteMgr.recipient",
        "emailAddress": {
          "@odata.type": "Microsoft.AADInviteMgr.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "messageLanguage": "Message Language value",
    "customizedMessageBody": "Customized Message Body value"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "https://example.com/inviteRedirectUrl/",
  "inviteRedeemUrl": "https://example.com/inviteRedeemUrl/",
  "status": "Status value",
  "resetRedemption": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.AADInviteMgr.invitation",
  "id": "2b9c89ee-89ee-2b9c-ee89-9c2bee899c2b",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "InvitedUserMessageInfo": {
    "@odata.type": "Microsoft.AADInviteMgr.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "Microsoft.AADInviteMgr.recipient",
        "emailAddress": {
          "@odata.type": "Microsoft.AADInviteMgr.emailAddress",
          "name": "Name value",
          "address": "Address value"
        }
      }
    ],
    "messageLanguage": "Message Language value",
    "customizedMessageBody": "Customized Message Body value"
  },
  "sendInvitationMessage": true,
  "inviteRedirectUrl": "https://example.com/inviteRedirectUrl/",
  "inviteRedeemUrl": "https://example.com/inviteRedeemUrl/",
  "status": "Status value",
  "resetRedemption": true
}
```

