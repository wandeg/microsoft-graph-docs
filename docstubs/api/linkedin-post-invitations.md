---
title: "Add invitations"
description: "Add invitations by posting to the invitations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add invitations

Namespace: microsoft.graph

Add invitations by posting to the invitations collection.

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
POST /linkedIn/invitations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [InvitationV2](../resources/invitationv2.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_invitationv2_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/linkedIn/invitations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.invitationv2"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 507

{
  "@odata.type": "#microsoft.graph.InvitationV2",
  "id": "dbf012ec-12ec-dbf0-ec12-f0dbec12f0db",
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

