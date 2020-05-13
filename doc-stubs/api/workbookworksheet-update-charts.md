---
title: "Update charts"
description: "Update the properties of a charts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update charts

Namespace: microsoft.graph

Update the properties of a charts object.

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
PATCH /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookChart](../resources/workbookchart.md) object.

The following table shows the properties that are required when you create the [workbookChart](../resources/workbookchart.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|height|Double|**TODO: Add Description**|
|left|Double|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|top|Double|**TODO: Add Description**|
|width|Double|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookChart](../resources/workbookchart.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_charts"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/charts
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.workbookChart",
  "height": "Double",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
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
  "@odata.type": "#microsoft.graph.workbookChart",
  "id": "22b4b3f5-b3f5-22b4-f5b3-b422f5b3b422",
  "height": "Double",
  "left": "Double",
  "name": "String",
  "top": "Double",
  "width": "Double"
}
```

