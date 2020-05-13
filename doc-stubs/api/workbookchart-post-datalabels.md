---
title: "Create dataLabels"
description: "Create a new dataLabels object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create dataLabels

Namespace: microsoft.graph

Create a new dataLabels object.

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
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object.

The following table shows the properties that are required when you create the [workbookChartDataLabels](../resources/workbookchartdatalabels.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|position|String|**TODO: Add Description**|
|separator|String|**TODO: Add Description**|
|showBubbleSize|Boolean|**TODO: Add Description**|
|showCategoryName|Boolean|**TODO: Add Description**|
|showLegendKey|Boolean|**TODO: Add Description**|
|showPercentage|Boolean|**TODO: Add Description**|
|showSeriesName|Boolean|**TODO: Add Description**|
|showValue|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookchartdatalabels_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/dataLabels
Content-Type: application/json
Content-length: 304

{
  "@odata.type": "#microsoft.graph.workbookChartDataLabels",
  "position": "String",
  "separator": "String",
  "showBubbleSize": "Boolean",
  "showCategoryName": "Boolean",
  "showLegendKey": "Boolean",
  "showPercentage": "Boolean",
  "showSeriesName": "Boolean",
  "showValue": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookchartdatalabels"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChartDataLabels",
  "id": "2bc57309-7309-2bc5-0973-c52b0973c52b",
  "position": "String",
  "separator": "String",
  "showBubbleSize": "Boolean",
  "showCategoryName": "Boolean",
  "showLegendKey": "Boolean",
  "showPercentage": "Boolean",
  "showSeriesName": "Boolean",
  "showValue": "Boolean"
}
```

