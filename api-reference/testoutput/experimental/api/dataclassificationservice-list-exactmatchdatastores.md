---
title: "List exactMatchDataStores"
description: "Get the exactMatchDataStores from the exactMatchDataStores navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List exactMatchDataStores

Namespace: microsoft.graph

Get the exactMatchDataStores from the exactMatchDataStores navigation property.

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
GET /dataClassification/exactMatchDataStores
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [exactMatchDataStore](../resources/exactmatchdatastore.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchdatastore"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/exactMatchDataStores
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchdatastore)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.exactMatchDataStore",
      "id": "0ecaed55-ed55-0eca-55ed-ca0e55edca0e",
      "displayName": "Display Name value",
      "description": "Description value",
      "dataLastUpdatedDateTime": "2016-12-31T23:57:12.7722306+03:00"
    }
  ]
}
```

