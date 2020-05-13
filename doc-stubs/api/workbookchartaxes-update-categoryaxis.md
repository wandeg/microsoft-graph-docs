---
title: "Update categoryAxis"
description: "Update the properties of a categoryAxis object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update categoryAxis

Namespace: microsoft.graph

Update the properties of a categoryAxis object.

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
PATCH /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartAxis](../resources/workbookchartaxis.md) object.

The following table shows the properties that are required when you create the [workbookChartAxis](../resources/workbookchartaxis.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|majorUnit|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|maximum|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|minimum|[Json](../resources/intune-json.md)|**TODO: Add Description**|
|minorUnit|[Json](../resources/intune-json.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookChartAxis](../resources/workbookchartaxis.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_categoryaxis"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis
Content-Type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
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
  "@odata.type": "#microsoft.graph.workbookChartAxis",
  "id": "9e1f8037-8037-9e1f-3780-1f9e37801f9e",
  "majorUnit": {
    "@odata.type": "microsoft.graph.Json"
  },
  "maximum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minimum": {
    "@odata.type": "microsoft.graph.Json"
  },
  "minorUnit": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

