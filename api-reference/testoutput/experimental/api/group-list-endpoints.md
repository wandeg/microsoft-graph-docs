---
title: "List endpoints"
description: "Get the endpoints from the endpoints navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List endpoints

Get the endpoints from the endpoints navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /groups/{groupsId}/endpoints
GET /me/joinedGroups/{groupId}/endpoints
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [endpoint](../resources/endpoint.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/groups/{groupsId}/endpoints
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.endpoint)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.endpoint",
      "id": "12485afa-5afa-1248-fa5a-4812fa5a4812",
      "deletedDateTime": "2017-01-01T00:00:34.0507931+03:00",
      "capability": "Capability value",
      "providerId": "Provider Id value",
      "providerName": "Provider Name value",
      "uri": "Uri value",
      "providerResourceId": "Provider Resource Id value"
    }
  ]
}
```

