---
title: "Get offerShiftRequest"
description: "Read the properties and relationships of an offerShiftRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get offerShiftRequest

Namespace: microsoft.graph

Read the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.

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
GET /teams/{teamsId}/schedule/offerShiftRequests/{offerShiftRequestId}
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

If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/schedule/offerShiftRequests/{offerShiftRequestId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.offerShiftRequest",
    "id": "b9e6dc81-dc81-b9e6-81dc-e6b981dce6b9",
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "assignedTo": "String",
    "state": "String",
    "senderMessage": "String",
    "senderDateTime": "String (timestamp)",
    "managerActionMessage": "String",
    "managerActionDateTime": "String (timestamp)",
    "senderUserId": "String",
    "managerUserId": "String",
    "recipientActionMessage": "String",
    "recipientActionDateTime": "String (timestamp)",
    "senderShiftId": "String",
    "recipientUserId": "String"
  }
}
```

