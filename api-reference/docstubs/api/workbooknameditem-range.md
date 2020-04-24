---
title: "workbookNamedItem: range"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# range

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/range
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/names/{workbookNamedItemId}/range
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [workbookRange](../resources/workbookrange.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "workbooknameditem_range"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/range
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrange"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.workbookRange",
    "id": "afb7dc09-dc09-afb7-09dc-b7af09dcb7af",
    "address": "Address value",
    "addressLocal": "Address Local value",
    "cellCount": 9,
    "columnCount": 11,
    "columnHidden": true,
    "columnIndex": 11,
    "formulas": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasLocal": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasR1C1": {
      "@odata.type": "microsoft.graph.Json"
    },
    "hidden": true,
    "numberFormat": {
      "@odata.type": "microsoft.graph.Json"
    },
    "rowCount": 8,
    "rowHidden": true,
    "rowIndex": 8,
    "text": {
      "@odata.type": "microsoft.graph.Json"
    },
    "valueTypes": {
      "@odata.type": "microsoft.graph.Json"
    },
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```

