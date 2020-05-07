---
title: "Create title"
description: "Create a new title object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create title

Namespace: microsoft.graph

Create a new title object.

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
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChartTitle](../resources/workbookcharttitle.md) object.

The following table shows the properties that are required when you create the [workbookChartTitle](../resources/workbookcharttitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|overlay|Boolean|**TODO: Add Description**|
|text|String|**TODO: Add Description**|
|visible|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookChartTitle](../resources/workbookcharttitle.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookcharttitle_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/title
Content-Type: application/json
Content-length: 131

{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "overlay": "Boolean",
  "text": "String",
  "visible": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookcharttitle"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChartTitle",
  "id": "40bc5ee7-5ee7-40bc-e75e-bc40e75ebc40",
  "overlay": "Boolean",
  "text": "String",
  "visible": "Boolean"
}
```

