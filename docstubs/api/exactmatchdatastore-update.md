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
Here is an example of the request.
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
  "dataLastUpdatedDateTime": "2016-12-31T23:59:49.8546729+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "e80c9c2e-9c2e-e80c-2e9c-0ce82e9c0ce8",
  "displayName": "Display Name value",
  "description": "Description value",
  "dataLastUpdatedDateTime": "2016-12-31T23:59:49.8546729+00:00"
}
```

