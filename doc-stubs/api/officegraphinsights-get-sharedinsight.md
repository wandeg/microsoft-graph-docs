---
title: "Get shared"
description: "Read the properties and relationships of a sharedInsight object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get shared

Namespace: microsoft.graph

Read the properties and relationships of a [sharedInsight](../resources/sharedinsight.md) object.

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
GET /users/{usersId}/insights/shared
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

If successful, this method returns a `200 OK` response code and a [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sharedinsight"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/insights/shared
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedInsight"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.sharedInsight",
    "id": "cdb03b69-3b69-cdb0-693b-b0cd693bb0cd",
    "lastShared": {
      "@odata.type": "microsoft.graph.sharingDetail"
    },
    "sharingHistory": [
      {
        "@odata.type": "microsoft.graph.sharingDetail"
      }
    ],
    "resourceVisualization": {
      "@odata.type": "microsoft.graph.resourceVisualization"
    },
    "resourceReference": {
      "@odata.type": "microsoft.graph.resourceReference"
    }
  }
}
```

