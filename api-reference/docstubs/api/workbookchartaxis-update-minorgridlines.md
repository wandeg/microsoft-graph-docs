---
title: "Update minorGridlines"
description: "Update the properties of a minorGridlines object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update minorGridlines

Namespace: microsoft.graph

Update the properties of a minorGridlines object.

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
PATCH /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/minorGridlines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [workbookChartGridlines](../resources/workbookchartgridlines.md) object.

The following table shows the properties that are required when you create the [workbookChartGridlines](../resources/workbookchartgridlines.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|visible|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartGridlines](../resources/workbookchartgridlines.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_minorgridlines"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/axes/categoryAxis/minorGridlines
Content-Type: application/json
Content-length: 84

{
  "@odata.type": "#microsoft.graph.workbookChartGridlines",
  "visible": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookChartGridlines",
  "id": "27b3fbe8-fbe8-27b3-e8fb-b327e8fbb327",
  "visible": true
}
```

