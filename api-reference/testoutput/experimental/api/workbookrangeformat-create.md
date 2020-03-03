---
title: "Create workbookRangeFormat"
description: "Create a new workbookRangeFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookRangeFormat

Namespace: microsoft.graph

Create a new [workbookRangeFormat](../resources/workbookrangeformat.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.workbookRangeFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookRangeFormat](../resources/workbookrangeformat.md) object.

The following table shows the properties that are required when you create the [workbookRangeFormat](../resources/workbookrangeformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|columnWidth|Double||
|horizontalAlignment|String||
|rowHeight|Double||
|verticalAlignment|String||
|wrapText|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookrangeformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeFormat not found
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "columnWidth": "Double",
  "horizontalAlignment": "Horizontal Alignment value",
  "rowHeight": "Double",
  "verticalAlignment": "Vertical Alignment value",
  "wrapText": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangeformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "id": "ce2c6c73-6c73-ce2c-736c-2cce736c2cce",
  "columnWidth": "Double",
  "horizontalAlignment": "Horizontal Alignment value",
  "rowHeight": "Double",
  "verticalAlignment": "Vertical Alignment value",
  "wrapText": true
}
```

