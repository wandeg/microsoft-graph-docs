---
title: "Update format"
description: "Update the properties of a format object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update format

Namespace: microsoft.graph

Update the properties of a format object.

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
PATCH /workbookRange/format
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookRangeFormat](../resources/workbookrangeformat.md) object.

The following table shows the properties that are required when you create the [workbookRangeFormat](../resources/workbookrangeformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|columnWidth|Double|**TODO: Add Description**|
|horizontalAlignment|String|**TODO: Add Description**|
|rowHeight|Double|**TODO: Add Description**|
|verticalAlignment|String|**TODO: Add Description**|
|wrapText|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_format"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/workbookRange/format
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "columnWidth": "Double",
  "horizontalAlignment": "String",
  "rowHeight": "Double",
  "verticalAlignment": "String",
  "wrapText": "Boolean"
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
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "id": "14b8fcee-fcee-14b8-eefc-b814eefcb814",
  "columnWidth": "Double",
  "horizontalAlignment": "String",
  "rowHeight": "Double",
  "verticalAlignment": "String",
  "wrapText": "Boolean"
}
```

