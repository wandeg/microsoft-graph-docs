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
|Authorization|Bearer {token}. Required|

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
      "id": "42789d05-9d05-4278-059d-7842059d7842",
      "userId": "User Id value",
      "userName": "User Name value",
      "userMail": "User Mail value",
      "roleId": "Role Id value",
      "roleName": "Role Name value",
      "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
      "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
      "requestorId": "Requestor Id value",
      "requestorName": "Requestor Name value",
      "tenantId": "Tenant Id value",
      "requestType": "Request Type value",
      "additionalInformation": "Additional Information value",
      "referenceKey": "Reference Key value",
      "referenceSystem": "Reference System value"
    }
  ]
}
```

