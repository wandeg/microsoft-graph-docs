---
title: "Update workbookChartAxisTitle"
description: "Update the properties of a workbookChartAxisTitle object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookChartAxisTitle

Update the properties of a [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookChartAxisTitle](../resources/workbookChartAxisTitle.md) object.

The following table shows the properties that are required when you create the [workbookChartAxisTitle](../resources/workbookchartaxistitle.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|visible|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartAxisTitle](../resources/workbookchartaxistitle.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookchartaxistitle"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/title
Content-type: application/json
Content-length: 109

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "text": "Text value",
  "visible": true
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
Content-Length: 158

{
  "@odata.type": "#microsoft.graph.workbookChartAxisTitle",
  "id": "6bd31bac-1bac-6bd3-ac1b-d36bac1bd36b",
  "text": "Text value",
  "visible": true
}
```

