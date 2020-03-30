---
title: "Get namedLocation"
description: "Read properties and relationships of the namedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get namedLocation

Namespace: microsoft.graph

Read properties and relationships of the [namedLocation](../resources/namedlocation.md) object.

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
GET /identity/conditionalAccess/namedLocations/{namedLocationId}
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
If successful, this method returns a `200 OK` response code and [namedLocation](../resources/namedlocation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/{namedLocationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "value": {
    "@odata.type": "#microsoft.graph.namedLocation",
    "id": "dd219c98-9c98-dd21-989c-21dd989c21dd",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "modifiedDateTime": "2016-12-31T23:57:56.5934914+03:00"
  }
}
```

