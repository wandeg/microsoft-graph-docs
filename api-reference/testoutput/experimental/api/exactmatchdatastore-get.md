---
title: "Get exactMatchDataStore"
description: "Read properties and relationships of the exactMatchDataStore object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get exactMatchDataStore

Read properties and relationships of the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

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
GET /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [exactMatchDataStore](../resources/exactmatchdatastore.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchdatastore"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchDataStore"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchDataStore",
    "id": "5100038f-038f-5100-8f03-00518f030051",
    "displayName": "Display Name value",
    "description": "Description value",
    "dataLastUpdatedDateTime": "2017-01-01T00:02:56.7657585+03:00"
  }
}
```

