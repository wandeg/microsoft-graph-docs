---
title: "List invitations"
description: "Get a list of the invitation objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List invitations

Namespace: Microsoft.AADInviteMgr

Get a list of the [invitation](../resources/invitation.md) objects and their properties.

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
GET /invitations
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
If successful, this method returns a `200 OK` response code and a collection of [invitation](../resources/invitation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_invitation"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.aadinvitemgr.invitation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

