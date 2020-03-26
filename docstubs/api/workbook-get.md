---
title: "Get workbook"
description: "Read properties and relationships of the workbook object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbook

Namespace: microsoft.graph

Read properties and relationships of the [workbook](../resources/workbook.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /workbooks/{workbooksId}/workbook
GET /me/drive/items/{driveItemId}/workbook
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [workbook](../resources/workbook.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbook"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbook"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 122

{
  "value": {
    "@odata.type": "#microsoft.graph.workbook",
    "id": "3a46d2a5-d2a5-3a46-a5d2-463aa5d2463a"
  }
}
```

