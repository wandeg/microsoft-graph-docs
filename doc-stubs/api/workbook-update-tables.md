---
title: "Update tables"
description: "Update the properties of a tables object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update tables

Namespace: microsoft.graph

Update the properties of a tables object.

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
PATCH /workbooks/{workbooksId}/workbook/tables
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookTable](../resources/workbooktable.md) object.

The following table shows the properties that are required when you create the [workbookTable](../resources/workbooktable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|highlightFirstColumn|Boolean|**TODO: Add Description**|
|highlightLastColumn|Boolean|**TODO: Add Description**|
|legacyId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|showBandedColumns|Boolean|**TODO: Add Description**|
|showBandedRows|Boolean|**TODO: Add Description**|
|showFilterButton|Boolean|**TODO: Add Description**|
|showHeaders|Boolean|**TODO: Add Description**|
|showTotals|Boolean|**TODO: Add Description**|
|style|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tables"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/tables
Content-Type: application/json
Content-length: 356

{
  "@odata.type": "#microsoft.graph.workbookTable",
  "highlightFirstColumn": "Boolean",
  "highlightLastColumn": "Boolean",
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": "Boolean",
  "showBandedRows": "Boolean",
  "showFilterButton": "Boolean",
  "showHeaders": "Boolean",
  "showTotals": "Boolean",
  "style": "String"
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
  "@odata.type": "#microsoft.graph.workbookTable",
  "id": "a67ec5bb-c5bb-a67e-bbc5-7ea6bbc57ea6",
  "highlightFirstColumn": "Boolean",
  "highlightLastColumn": "Boolean",
  "legacyId": "String",
  "name": "String",
  "showBandedColumns": "Boolean",
  "showBandedRows": "Boolean",
  "showFilterButton": "Boolean",
  "showHeaders": "Boolean",
  "showTotals": "Boolean",
  "style": "String"
}
```

