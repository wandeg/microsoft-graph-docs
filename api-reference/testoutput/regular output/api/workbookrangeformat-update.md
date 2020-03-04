---
title: "Update workbookRangeFormat"
description: "Update the properties of a workbookRangeFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRangeFormat

Namespace: microsoft.graph

Update the properties of a [workbookRangeFormat](../resources/workbookrangeformat.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookRangeFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
If successful, this method returns a `200 OK` response code and an updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrangeformat"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeFormat not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.workbookRangeFormat",
  "id": "57aff004-f004-57af-04f0-af5704f0af57",
  "columnWidth": "Double",
  "horizontalAlignment": "Horizontal Alignment value",
  "rowHeight": "Double",
  "verticalAlignment": "Vertical Alignment value",
  "wrapText": true
}
```

