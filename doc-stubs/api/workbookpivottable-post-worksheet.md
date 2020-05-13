---
title: "Create worksheet"
description: "Create a new worksheet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create worksheet

Namespace: microsoft.graph

Create a new worksheet object.

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
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/{workbookPivotTableId}/worksheet
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookWorksheet](../resources/workbookworksheet.md) object.

The following table shows the properties that are required when you create the [workbookWorksheet](../resources/workbookworksheet.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|position|Int32|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookworksheet_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/pivotTables/{workbookPivotTableId}/worksheet
Content-Type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "name": "String",
  "position": "Integer",
  "visibility": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookworksheet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "e8a15c54-5c54-e8a1-545c-a1e8545ca1e8",
  "name": "String",
  "position": "Integer",
  "visibility": "String"
}
```

