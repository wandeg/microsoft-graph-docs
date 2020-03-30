---
title: "Update InvitationV2"
description: "Update the properties of a InvitationV2 object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update InvitationV2

Namespace: microsoft.graph

Update the properties of a [InvitationV2](../resources/invitationv2.md) object.

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
PATCH /linkedIn/invitations/{InvitationV2Id}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [InvitationV2](../resources/invitationv2.md) object.

The following table shows the properties that are required when you create the [InvitationV2](../resources/invitationv2.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|created|Int64||
|lastModified|Int64||
|inviter|String||
|invitee|String||
|message|[InvitationV2Message](../resources/invitationv2message.md)||
|trackingId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [InvitationV2](../resources/invitationv2.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_invitationv2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/linkedIn/invitations/{InvitationV2Id}
Content-type: application/json
Content-length: 458

{
  "@odata.type": "#microsoft.graph.InvitationV2",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 507

{
  "@odata.type": "#microsoft.graph.InvitationV2",
  "id": "86bcd09e-d09e-86bc-9ed0-bc869ed0bc86",
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
```

