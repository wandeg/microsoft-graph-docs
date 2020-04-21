---
title: "Get invitation"
description: "Read properties and relationships of an invitation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get invitation

Namespace: microsoft.graph

Read properties and relationships of an [invitation](../resources/invitation.md) object.

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
GET /invitations/{invitationsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [invitation](../resources/invitation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_invitation"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.invitation",
    "id": "6651153e-153e-6651-3e15-51663e155166",
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
    "status": "Status value"
  }
}
```

