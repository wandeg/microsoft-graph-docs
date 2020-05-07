---
title: "List reviewSets"
description: "Get the reviewSets from the reviewSets navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List reviewSets

Namespace: microsoft.graph

Get the reviewSets from the reviewSets navigation property.

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
GET /cases/{casesId}/reviewSets
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

If successful, this method returns a `200 OK` response code and a collection of [reviewSet](../resources/reviewset.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_reviewset"
}
-->
``` http
GET https://graph.microsoft.com/beta/cases/{casesId}/reviewSets
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.compliance.ediscovery.contract.reviewset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.compliance.ediscovery.contract.reviewSet",
      "createdBy": "String",
      "id": "51b6280d-280d-51b6-0d28-b6510d28b651",
      "displayName": "String",
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```

