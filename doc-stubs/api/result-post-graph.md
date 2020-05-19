---
title: "Create Result"
description: "Create a new Result object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create Result

Namespace: microsoft.graph

Create a new [Result](../resources/result.md) object.

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
POST /graph
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [Result](../resources/result.md) object.

The following table shows the properties that are required when you create the [Result](../resources/result.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|entities|[ResultEntities](../resources/resultentities.md)|**TODO: Add Description**|
|aggregations|[LIAggregations](../resources/liaggregations.md) collection|**TODO: Add Description**|
|metadata|[Metadata](../resources/metadata.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [Result](../resources/result.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_result_from_graph"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/graph
Content-Type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.Result",
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
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.result"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.Result",
  "id": "3bf96446-6446-3bf9-4664-f93b4664f93b",
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
```

