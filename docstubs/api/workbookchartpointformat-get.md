---
title: "Get workbookChartPointFormat"
description: "Read properties and relationships of the workbookChartPointFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookChartPointFormat

Namespace: microsoft.graph

Read properties and relationships of the [workbookChartPointFormat](../resources/workbookchartpointformat.md) object.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/{workbookChartPointId}/format
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
If successful, this method returns a `200 OK` response code and [workbookChartPointFormat](../resources/workbookchartpointformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookchartpointformat"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/series/{workbookChartSeriesId}/points/{workbookChartPointId}/format
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 138

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookChartPointFormat",
    "id": "d5ec5a0d-5a0d-d5ec-0d5a-ecd50d5aecd5"
  }
}
```

