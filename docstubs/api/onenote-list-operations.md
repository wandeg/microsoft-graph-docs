---
title: "List operations"
description: "Get the onenoteOperations from the operations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List operations

Namespace: microsoft.graph

Get the onenoteOperations from the operations navigation property.

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
GET /me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
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
If successful, this method returns a `200 OK` response code and a collection of [onenoteOperation](../resources/onenoteoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/sites/{siteId}/onenote/operations
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
Content-Length: 612

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenoteOperation",
      "id": "3ad0ca5e-ca5e-3ad0-5eca-d03a5ecad03a",
      "status": "String",
      "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
      "lastActionDateTime": "2017-01-01T00:00:14.9774895+03:00",
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

