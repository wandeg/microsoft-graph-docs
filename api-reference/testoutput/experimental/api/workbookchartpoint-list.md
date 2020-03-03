---
title: "List workbookChartPoints"
description: "List properties and relationships of the workbookChartPoint objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookChartPoints

Namespace: microsoft.graph

List properties and relationships of the [workbookChartPoint](../resources/workbookchartpoint.md) objects.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookChartPoint](../resources/workbookchartpoint.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookchartpoint"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookchartpoint)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 225

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookChartPoint",
      "id": "0c611f4a-1f4a-0c61-4a1f-610c4a1f610c",
      "value": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```

