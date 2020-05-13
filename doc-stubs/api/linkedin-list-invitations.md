---
title: "List invitations"
description: "Get the InvitationV2 from the invitations navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List invitations

Namespace: microsoft.graph

Get the InvitationV2 from the invitations navigation property.

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
GET /linkedIn/invitations
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [InvitationV2](../resources/invitationv2.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_invitationv2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/linkedIn/invitations
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.invitationv2)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.InvitationV2",
      "id": "cf38e414-e414-cf38-14e4-38cf14e438cf",
      "created": "Integer",
      "lastModified": "Integer",
      "inviter": "String",
      "invitee": "String",
      "message": {
        "@odata.type": "microsoft.graph.InvitationV2Message"
      },
      "trackingId": "String"
    }
  ]
}
```

