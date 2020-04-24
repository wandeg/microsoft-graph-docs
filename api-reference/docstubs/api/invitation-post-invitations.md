---
title: "Create invitation"
description: "Create a new invitation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create invitation

Namespace: microsoft.graph

Create a new [invitation](../resources/invitation.md) object.

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
POST /invitations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [invitation](../resources/invitation.md) object.

The following table shows the properties that are required when you create the [invitation](../resources/invitation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invitedUserDisplayName|String|**TODO: Add Description**|
|invitedUserType|String|**TODO: Add Description**|
|invitedUserEmailAddress|String|**TODO: Add Description**|
|invitedUserMessageInfo|[invitedUserMessageInfo](../resources/invitedusermessageinfo.md)|**TODO: Add Description**|
|sendInvitationMessage|Boolean|**TODO: Add Description**|
|inviteRedirectUrl|String|**TODO: Add Description**|
|inviteRedeemUrl|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|resetRedemption|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [invitation](../resources/invitation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_invitation_from_invitations"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json
Content-length: 930

{
  "@odata.type": "#microsoft.graph.invitation",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.invitation",
  "id": "3c88db8e-db8e-3c88-8edb-883c8edb883c",
  "invitedUserDisplayName": "Invited User Display Name value",
  "invitedUserType": "Invited User Type value",
  "invitedUserEmailAddress": "Invited User Email Address value",
  "invitedUserMessageInfo": {
    "@odata.type": "microsoft.graph.invitedUserMessageInfo",
    "ccRecipients": [
      {
        "@odata.type": "microsoft.graph.recipient",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
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

