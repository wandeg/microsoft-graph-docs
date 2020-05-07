---
title: "Get workbookChartFill"
description: "Read the properties and relationships of a workbookChartFill object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get workbookChartFill

Namespace: microsoft.graph

Read the properties and relationships of a [workbookChartFill](../resources/workbookchartfill.md) object.

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
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/fill
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title/format/fill
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/legend/format/fill
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels/format/fill
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/format/fill
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/{workbookChartPointId}/format/fill
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

If successful, this method returns a `200 OK` response code and a [workbookChartFill](../resources/workbookchartfill.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookchartfill"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/fill
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFill"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.workbookChartFill",
    "id": "5c7c2bb8-2bb8-5c7c-b82b-7c5cb82b7c5c"
  }
}
```

