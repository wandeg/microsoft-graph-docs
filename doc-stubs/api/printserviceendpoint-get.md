---
title: "Get printServiceEndpoint"
description: "Read the properties and relationships of a printServiceEndpoint object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get printServiceEndpoint

Namespace: microsoft.graph

Read the properties and relationships of a [printServiceEndpoint](../resources/printserviceendpoint.md) object.

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
GET /print/services/{printServiceId}/endpoints/{printServiceEndpointId}
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

If successful, this method returns a `200 OK` response code and a [printServiceEndpoint](../resources/printserviceendpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/services/{printServiceId}/endpoints/{printServiceEndpointId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.printServiceEndpoint",
    "id": "1a4a8a35-8a35-1a4a-358a-4a1a358a4a1a",
    "displayName": "String",
    "uri": "String"
  }
}
```

