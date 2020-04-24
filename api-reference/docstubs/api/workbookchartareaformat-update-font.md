---
title: "Update font"
description: "Update the properties of a font object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update font

Namespace: microsoft.graph

Update the properties of a font object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/font
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookChartFont](../resources/workbookchartfont.md) object.

The following table shows the properties that are required when you create the [workbookChartFont](../resources/workbookchartfont.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|bold|Boolean|**TODO: Add Description**|
|color|String|**TODO: Add Description**|
|italic|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|size|Double|**TODO: Add Description**|
|underline|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookChartFont](../resources/workbookchartfont.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_font"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/charts/{workbookChartId}/format/font
Content-Type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.workbookChartFont",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
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
  "@odata.type": "#microsoft.graph.workbookChartFont",
  "id": "140dce12-ce12-140d-12ce-0d1412ce0d14",
  "bold": true,
  "color": "Color value",
  "italic": true,
  "name": "Name value",
  "size": "Double",
  "underline": "Underline value"
}
```

