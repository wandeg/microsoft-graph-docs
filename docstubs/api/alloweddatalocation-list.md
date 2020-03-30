---
title: "List allowedDataLocations"
description: "List properties and relationships of the allowedDataLocation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List allowedDataLocations

Namespace: microsoft.graph

List properties and relationships of the [allowedDataLocation](../resources/alloweddatalocation.md) objects.

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
GET /allowedDataLocations
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
If successful, this method returns a `200 OK` response code and a collection of [allowedDataLocation](../resources/alloweddatalocation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_alloweddatalocation"
}
-->
``` http
GET https://graph.microsoft.com/beta/allowedDataLocations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.alloweddatalocation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.allowedDataLocation",
      "id": "513476df-76df-5134-df76-3451df763451",
      "appId": "App Id value",
      "location": "Location value",
      "isDefault": true,
      "domain": "Domain value"
    }
  ]
}
```

