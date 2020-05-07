---
title: "Create queries"
description: "Create a new queries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create queries

Namespace: microsoft.graph

Create a new queries object.

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
POST /cases/{casesId}/reviewSets/{reviewSetId}/queries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [reviewSetQuery](../resources/reviewsetquery.md) object.

The following table shows the properties that are required when you create the [reviewSetQuery](../resources/reviewsetquery.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|query|String|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_reviewsetquery_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/cases/{casesId}/reviewSets/{reviewSetId}/queries
Content-Type: application/json
Content-length: 132

{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
  "query": "String",
  "createdBy": "String",
  "displayName": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewsetquery"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
  "id": "5ac11718-1718-5ac1-1817-c15a1817c15a",
  "query": "String",
  "lastModifiedBy": "String",
  "createdBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

