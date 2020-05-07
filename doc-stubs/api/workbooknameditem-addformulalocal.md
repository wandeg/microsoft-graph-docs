---
title: "workbookNamedItem: addFormulaLocal"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# addFormulaLocal

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /workbooks/{workbooksId}/workbook/names/addFormulaLocal
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/names/addFormulaLocal
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|name|String|**TODO: Add Description**|
|formula|String|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [workbookNamedItem](../resources/workbooknameditem.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbooknameditem_addformulalocal"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/addFormulaLocal

Content-Type: application/json
Content-length: 72

{
  "name": "String",
  "formula": "String",
  "comment": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooknameditem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "id": "String (identifier)",
    "comment": "String",
    "name": "String",
    "scope": "String",
    "type": "String",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    },
    "visible": "Boolean"
  }
}
```

