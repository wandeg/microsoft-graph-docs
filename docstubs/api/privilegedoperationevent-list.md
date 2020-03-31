---
title: "List privilegedOperationEvents"
description: "List properties and relationships of the privilegedOperationEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedOperationEvents

Namespace: microsoft.graph

List properties and relationships of the [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects.

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
GET /privilegedOperationEvents
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
If successful, this method returns a `200 OK` response code and a collection of [privilegedOperationEvent](../resources/privilegedoperationevent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedoperationevent"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedOperationEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedoperationevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 804

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedOperationEvent",
      "id": "d639bc40-bc40-d639-40bc-39d640bc39d6",
      "userId": "User Id value",
      "userName": "User Name value",
      "userMail": "User Mail value",
      "roleId": "Role Id value",
      "roleName": "Role Name value",
      "expirationDateTime": "2016-12-31T23:56:49.0349895+03:00",
      "creationDateTime": "2016-12-31T23:58:37.0462827+03:00",
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

