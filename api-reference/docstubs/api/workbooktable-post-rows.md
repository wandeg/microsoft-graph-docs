---
title: "Create rows"
description: "Create a new rows object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create rows

Namespace: microsoft.graph

Create a new rows object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookTableRow](../resources/workbooktablerow.md) object.

The following table shows the properties that are required when you create the [workbookTableRow](../resources/workbooktablerow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|index|Int32|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workbookTableRow](../resources/workbooktablerow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktablerow_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "index": 5,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktablerow"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "id": "e0cb97f9-97f9-e0cb-f997-cbe0f997cbe0",
  "index": 5,
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

