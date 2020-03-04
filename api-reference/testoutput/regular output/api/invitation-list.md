---
title: "List invitations"
description: "List properties and relationships of the invitation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List invitations

Namespace: microsoft.graph

List properties and relationships of the [invitation](../resources/invitation.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /invitations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [invitation](../resources/invitation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_invitation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/invitations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.invitation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1080

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.invitation",
      "id": "4fc57730-7730-4fc5-3077-c54f3077c54f",
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
  ]
}
```

