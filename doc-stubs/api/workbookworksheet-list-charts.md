---
title: "List charts"
description: "Get the workbookCharts from the charts navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List charts

Namespace: microsoft.graph

Get the workbookCharts from the charts navigation property.

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
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts
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

If successful, this method returns a `200 OK` response code and a collection of [workbookChart](../resources/workbookchart.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookchart"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookchart)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookChart",
      "id": "2baa6da8-6da8-2baa-a86d-aa2ba86daa2b",
      "height": "Double",
      "left": "Double",
      "name": "String",
      "top": "Double",
      "width": "Double"
    }
  ]
}
```

