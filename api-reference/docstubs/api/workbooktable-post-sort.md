---
title: "Create sort"
description: "Create a new sort object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create sort

Namespace: microsoft.graph

Create a new sort object.

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
POST /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [workbookTableSort](../resources/workbooktablesort.md) object.

The following table shows the properties that are required when you create the [workbookTableSort](../resources/workbooktablesort.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|fields|[workbookSortField](../resources/workbooksortfield.md) collection|**TODO: Add Description**|
|matchCase|Boolean|**TODO: Add Description**|
|method|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workbookTableSort](../resources/workbooktablesort.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktablesort_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/sort
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktablesort"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookTableSort",
  "id": "84104302-4302-8410-0243-108402431084",
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

