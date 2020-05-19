---
title: "Create borders"
description: "Create a new borders object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create borders

Namespace: microsoft.graph

Create a new borders object.

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
POST /workbookRange/format/borders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeBorder](../resources/workbookrangeborder.md) object.

The following table shows the properties that are required when you create the [workbookRangeBorder](../resources/workbookrangeborder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|color|String|**TODO: Add Description**|
|sideIndex|String|**TODO: Add Description**|
|style|String|**TODO: Add Description**|
|weight|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookrangeborder_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/workbookRange/format/borders
Content-Type: application/json
Content-length: 154

{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "color": "String",
  "sideIndex": "String",
  "style": "String",
  "weight": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangeborder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "id": "3dc7fa0c-fa0c-3dc7-0cfa-c73d0cfac73d",
  "color": "String",
  "sideIndex": "String",
  "style": "String",
  "weight": "String"
}
```

