---
title: "List onenoteOperations"
description: "List properties and relationships of the onenoteOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onenoteOperations

Namespace: microsoft.graph

List properties and relationships of the [onenoteOperation](../resources/onenoteoperation.md) objects.

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
GET /me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenoteOperation](../resources/onenoteoperation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenoteoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenoteOperation",
      "id": "3ef37e7a-7e7a-3ef3-7a7e-f33e7a7ef33e",
      "status": "String",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastActionDateTime": "2016-12-31T23:56:52.9868016+03:00",
      "resourceLocation": "Resource Location value",
      "resourceId": "Resource Id value",
      "error": {
        "@odata.type": "microsoft.graph.onenoteOperationError",
        "code": "Code value",
        "message": "Message value"
      },
      "percentComplete": "Percent Complete value"
    }
  ]
}
```

