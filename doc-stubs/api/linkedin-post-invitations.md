---
title: "Create invitations"
description: "Create a new invitations object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create invitations

Namespace: microsoft.graph

Create a new invitations object.

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
POST /linkedIn/invitations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [InvitationV2](../resources/invitationv2.md) object.

The following table shows the properties that are required when you create the [InvitationV2](../resources/invitationv2.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|created|Int64|**TODO: Add Description**|
|lastModified|Int64|**TODO: Add Description**|
|inviter|String|**TODO: Add Description**|
|invitee|String|**TODO: Add Description**|
|message|[InvitationV2Message](../resources/invitationv2message.md)|**TODO: Add Description**|
|trackingId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [InvitationV2](../resources/invitationv2.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_invitationv2_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/linkedIn/invitations
Content-Type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.InvitationV2",
  "created": "Integer",
  "lastModified": "Integer",
  "inviter": "String",
  "invitee": "String",
  "message": {
    "@odata.type": "microsoft.graph.InvitationV2Message"
  },
  "trackingId": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitationv2"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.InvitationV2",
  "id": "c6443338-3338-c644-3833-44c6383344c6",
  "created": "Integer",
  "lastModified": "Integer",
  "inviter": "String",
  "invitee": "String",
  "message": {
    "@odata.type": "microsoft.graph.InvitationV2Message"
  },
  "trackingId": "String"
}
```

