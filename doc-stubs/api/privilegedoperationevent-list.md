---
title: "List privilegedOperationEvents"
description: "Get a list of the privilegedOperationEvent objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List privilegedOperationEvents
Namespace: microsoft.graph

Get a list of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects and their properties.

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
GET /privilegedOperationEvents
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

If successful, this method returns a `200 OK` response code and a collection of [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_privilegedoperationevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedOperationEvents
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedoperationevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedOperationEvent",
      "id": "144da38e-a38e-144d-8ea3-4d148ea34d14",
      "userId": "String",
      "userName": "String",
      "userMail": "String",
      "roleId": "String",
      "roleName": "String",
      "expirationDateTime": "String (timestamp)",
      "creationDateTime": "String (timestamp)",
      "requestorId": "String",
      "requestorName": "String",
      "tenantId": "String",
      "requestType": "String",
      "additionalInformation": "String",
      "referenceKey": "String",
      "referenceSystem": "String"
    }
  ]
}
```

