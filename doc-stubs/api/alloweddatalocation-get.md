---
title: "Get allowedDataLocation"
description: "Read the properties and relationships of an allowedDataLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get allowedDataLocation
Namespace: microsoft.graph

Read the properties and relationships of an [allowedDataLocation](../resources/alloweddatalocation.md) object.

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
GET /allowedDataLocations/{allowedDataLocationsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [allowedDataLocation](../resources/alloweddatalocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_alloweddatalocation"
}
-->
``` http
GET https://graph.microsoft.com/beta/allowedDataLocations/{allowedDataLocationsId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.allowedDataLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.allowedDataLocation",
    "id": "bc07a5e3-a5e3-bc07-e3a5-07bce3a507bc",
    "appId": "String",
    "location": "String",
    "isDefault": "Boolean",
    "domain": "String"
  }
}
```

