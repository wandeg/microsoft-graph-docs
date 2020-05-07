---
title: "Update exactMatchDataStores"
description: "Update the properties of an exactMatchDataStores object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update exactMatchDataStores

Namespace: microsoft.graph

Update the properties of an exactMatchDataStores object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/exactMatchDataStores
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [exactMatchDataStore](../resources/exactmatchdatastore.md) object.

The following table shows the properties that are required when you create the [exactMatchDataStore](../resources/exactmatchdatastore.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|dataLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [exactMatchDataStore](../resources/exactmatchdatastore.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_exactmatchdatastores"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/exactMatchDataStores
Content-Type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "displayName": "String",
  "description": "String",
  "dataLastUpdatedDateTime": "String (timestamp)"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.exactMatchDataStore",
  "id": "993c87b0-87b0-993c-b087-3c99b0873c99",
  "displayName": "String",
  "description": "String",
  "dataLastUpdatedDateTime": "String (timestamp)"
}
```

