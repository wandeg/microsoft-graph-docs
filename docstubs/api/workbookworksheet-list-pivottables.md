---
title: "List pivotTables"
description: "Get the workbookPivotTables from the pivotTables navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List pivotTables

Namespace: microsoft.graph

Get the workbookPivotTables from the pivotTables navigation property.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/pivotTables
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
If successful, this method returns a `200 OK` response code and a collection of [workbookPivotTable](../resources/workbookpivottable.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookpivottable"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/pivotTables
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookpivottable)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 179

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookPivotTable",
      "id": "328c37ef-37ef-328c-ef37-8c32ef378c32",
      "name": "Name value"
    }
  ]
}
```

