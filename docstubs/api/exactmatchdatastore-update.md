---
title: "Update exactMatchDataStore"
description: "Update the properties of a exactMatchDataStore object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update exactMatchDataStore

Namespace: microsoft.graph

Update the properties of a [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

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
PATCH /dataClassification/exactMatchDataStores/{exactMatchDataStoreId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

The following table shows the properties that are required when you create the [exactMatchDataStore](../resources/exactmatchdatastore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|String||
|dataLastUpdatedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [exactMatchDataStore](../resources/exactmatchdatastore.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_exactmatchdatastore"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores/{exactMatchDataStoreId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "displayName": "Display Name value",
  "description": "Description value",
  "dataLastUpdatedDateTime": "2017-01-01T00:00:39.8589537+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "id": "adb7b4f2-b4f2-adb7-f2b4-b7adf2b4b7ad",
  "displayName": "Display Name value",
  "description": "Description value",
  "dataLastUpdatedDateTime": "2017-01-01T00:00:39.8589537+00:00"
}
```

