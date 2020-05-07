---
title: "Get workbookWorksheet"
description: "Read the properties and relationships of a workbookWorksheet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get workbookWorksheet

Namespace: microsoft.graph

Read the properties and relationships of a [workbookWorksheet](../resources/workbookworksheet.md) object.

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
GET /workbooks/{workbooksId}/workbook/worksheets/{workbookWorksheetId}
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/worksheet
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/worksheet
GET /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/{workbookPivotTableId}/worksheet
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

If successful, this method returns a `200 OK` response code and a [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheet"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/worksheets/{workbookWorksheetId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.workbookWorksheet",
    "id": "e6a3ec10-ec10-e6a3-10ec-a3e610eca3e6",
    "name": "String",
    "position": "Integer",
    "visibility": "String"
  }
}
```

