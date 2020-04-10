---
title: "Get InvitationV2"
description: "Read properties and relationships of the InvitationV2 object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get InvitationV2

Namespace: microsoft.graph

Read properties and relationships of the [InvitationV2](../resources/invitationv2.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /linkedIn/invitations/{InvitationV2Id}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [InvitationV2](../resources/invitationv2.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_invitationv2"
}
-->
``` http
GET https://graph.microsoft.com/beta/linkedIn/invitations/{InvitationV2Id}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.InvitationV2"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": {
    "@odata.type": "#microsoft.graph.InvitationV2",
    "id": "a9b72e58-2e58-a9b7-582e-b7a9582eb7a9",
    "created": 7,
    "lastModified": 12,
    "inviter": "Inviter value",
    "invitee": "Invitee value",
    "message": {
      "@odata.type": "microsoft.graph.InvitationV2Message",
      "invitationTemplateID": "Invitation Template ID value",
      "invitationMessage": {
        "@odata.type": "microsoft.graph.InvitationMessage",
        "body": "Body value"
      }
    },
    "trackingId": "Tracking Id value"
  }
}
```

