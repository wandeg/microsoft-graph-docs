---
title: "List namedLocations"
description: "Get the namedLocations from the namedLocations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List namedLocations

Namespace: microsoft.graph

Get the namedLocations from the namedLocations navigation property.

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
GET /identity/conditionalAccess/namedLocations
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
If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.namedlocation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.namedLocation",
      "id": "ced29eff-9eff-ced2-ff9e-d2ceff9ed2ce",
      "displayName": "Display Name value",
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "modifiedDateTime": "2016-12-31T23:59:25.7728733+03:00"
    }
  ]
}
```

