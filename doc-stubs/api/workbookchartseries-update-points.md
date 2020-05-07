---
title: "Update points"
description: "Update the properties of a points object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update points

Namespace: microsoft.graph

Update the properties of a points object.

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
PATCH /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartPoint](../resources/workbookchartpoint.md) object.

The following table shows the properties that are required when you create the [workbookChartPoint](../resources/workbookchartpoint.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|value|[Json](../resources/json.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookChartPoint](../resources/workbookchartpoint.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_points"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points
Content-Type: application/json
Content-length: 123

{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChartPoint",
  "id": "bcbfd98b-d98b-bcbf-8bd9-bfbc8bd9bfbc",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

