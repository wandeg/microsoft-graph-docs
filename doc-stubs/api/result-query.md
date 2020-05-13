---
title: "Result: query"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# query

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /graph/query
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|queryId|String|**TODO: Add Description**|
|queryParams|[StringMapElement](../resources/stringmapelement.md) collection|**TODO: Add Description**|



## Response

If successful, this function returns a `200 OK` response code and a [Result](../resources/result.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "result_query"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/graph/query(queryId='parameterValue',queryParams=[
  {
    "@odata.type": "microsoft.graph.StringMapElement"
  }
])
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.result)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.Result",
      "id": "String (identifier)",
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
  ]
}
```

