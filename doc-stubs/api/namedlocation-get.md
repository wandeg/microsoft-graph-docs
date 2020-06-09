---
title: "Get namedLocation"
description: "Read the properties and relationships of a namedLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get namedLocation
Namespace: microsoft.graph

Read the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.

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
GET /identity/conditionalAccess/namedLocations/{namedLocationId}
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

If successful, this method returns a `200 OK` response code and a [namedLocation](../resources/namedlocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/{namedLocationId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.namedLocation",
    "id": "e013c6e6-c6e6-e013-e6c6-13e0e6c613e0",
    "displayName": "String",
    "createdDateTime": "String (timestamp)",
    "modifiedDateTime": "String (timestamp)"
  }
}
```

