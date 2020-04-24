---
title: "Update sort"
description: "Update the properties of a sort object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update sort

Namespace: microsoft.graph

Update the properties of a sort object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookTableSort](../resources/workbooktablesort.md) object.

The following table shows the properties that are required when you create the [workbookTableSort](../resources/workbooktablesort.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|fields|[workbookSortField](../resources/workbooksortfield.md) collection|**TODO: Add Description**|
|matchCase|Boolean|**TODO: Add Description**|
|method|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookTableSort](../resources/workbooktablesort.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sort"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
Content-Type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField",
      "ascending": true,
      "color": "Color value",
      "dataOption": "Data Option value",
      "icon": {
        "@odata.type": "microsoft.graph.workbookIcon",
        "index": 5,
        "set": "Set value"
      },
      "key": 3,
      "sortOn": "Sort On value"
    }
  ],
  "matchCase": true,
  "method": "Method value"
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
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "id": "e002f394-f394-e002-94f3-02e094f302e0",
  "fields": [
    {
      "@odata.type": "microsoft.graph.workbookSortField",
      "ascending": true,
      "color": "Color value",
      "dataOption": "Data Option value",
      "icon": {
        "@odata.type": "microsoft.graph.workbookIcon",
        "index": 5,
        "set": "Set value"
      },
      "key": 3,
      "sortOn": "Sort On value"
    }
  ],
  "matchCase": true,
  "method": "Method value"
}
```

