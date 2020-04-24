---
title: "Update columns"
description: "Update the properties of a columns object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update columns

Namespace: microsoft.graph

Update the properties of a columns object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookTableColumn](../resources/workbooktablecolumn.md) object.

The following table shows the properties that are required when you create the [workbookTableColumn](../resources/workbooktablecolumn.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|index|Int32|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_columns"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
Content-Type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "index": 5,
  "name": "Name value",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
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
  "@odata.type": "#microsoft.graph.workbookTableColumn",
  "id": "b5b00ef1-0ef1-b5b0-f10e-b0b5f10eb0b5",
  "index": 5,
  "name": "Name value",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

