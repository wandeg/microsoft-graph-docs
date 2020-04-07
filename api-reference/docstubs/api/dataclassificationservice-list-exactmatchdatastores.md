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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /dataClassification/exactMatchDataStores
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
If successful, this method returns a `200 OK` response code and a collection of [exactMatchDataStore](../resources/exactmatchdatastore.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchdatastore"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores
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
      "id": "649a798a-798a-649a-8a79-9a648a799a64",
      "displayName": "Display Name value",
      "description": "Description value",
      "dataLastUpdatedDateTime": "2017-01-01T00:03:28.5386576+03:00"
    }
  ]
}
```

