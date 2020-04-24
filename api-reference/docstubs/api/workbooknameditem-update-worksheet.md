---
title: "Update worksheet"
description: "Update the properties of a worksheet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update worksheet

Namespace: microsoft.graph

Update the properties of a worksheet object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookWorksheet](../resources/workbookworksheet.md) object.

The following table shows the properties that are required when you create the [workbookWorksheet](../resources/workbookworksheet.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|position|Int32|**TODO: Add Description**|
|visibility|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookWorksheet](../resources/workbookworksheet.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet
Content-Type: application/json
Content-length: 139

{
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
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
  "@odata.type": "#microsoft.graph.workbookWorksheet",
  "id": "c5a59ce6-9ce6-c5a5-e69c-a5c5e69ca5c5",
  "name": "Name value",
  "position": 8,
  "visibility": "Visibility value"
}
```

