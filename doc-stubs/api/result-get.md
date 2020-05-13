---
title: "Get Result"
description: "Read the properties and relationships of a Result object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get Result

Namespace: microsoft.graph

Read the properties and relationships of a [Result](../resources/result.md) object.

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
GET /graph/{graphId}
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

If successful, this method returns a `200 OK` response code and a [Result](../resources/result.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_result"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/graph/{graphId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Result"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.Result",
    "id": "ccd9d40c-d40c-ccd9-0cd4-d9cc0cd4d9cc",
    "entities": {
      "@odata.type": "microsoft.graph.ResultEntities"
    },
    "aggregations": [
      {
        "@odata.type": "microsoft.graph.LIAggregations"
      }
    ],
    "metadata": {
      "@odata.type": "microsoft.graph.Metadata"
    }
  }
}
```

