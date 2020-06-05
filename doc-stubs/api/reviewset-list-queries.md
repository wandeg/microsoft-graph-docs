---
title: "List queries"
description: "Get the reviewSetQueries from the queries navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List queries
Namespace: microsoft.graph

Get the reviewSetQueries from the queries navigation property.

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
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/reviewSets/{reviewSetId}/queries
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

If successful, this method returns a `200 OK` response code and a collection of [reviewSetQuery](../resources/reviewsetquery.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}
-->
``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/reviewSets/{reviewSetId}/queries
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.reviewsetquery)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.reviewSetQuery",
      "id": "9add114b-114b-9add-4b11-dd9a4b11dd9a",
      "query": "String",
      "lastModifiedBy": "String",
      "createdBy": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "displayName": "String",
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```

