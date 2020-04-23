---
title: "Create tables"
description: "Create a new tables object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create tables

Namespace: microsoft.graph

Create a new tables object.

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
POST /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/tables
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookTable](../resources/workbooktable.md) object.

The following table shows the properties that are required when you create the [workbookTable](../resources/workbooktable.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|highlightFirstColumn|Boolean|**TODO: Add Description**|
|highlightLastColumn|Boolean|**TODO: Add Description**|
|legacyId|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|showBandedColumns|Boolean|**TODO: Add Description**|
|showBandedRows|Boolean|**TODO: Add Description**|
|showFilterButton|Boolean|**TODO: Add Description**|
|showHeaders|Boolean|**TODO: Add Description**|
|showTotals|Boolean|**TODO: Add Description**|
|style|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workbookTable](../resources/workbooktable.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbooktable_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/tables
Content-Type: application/json
Content-length: 339

{
  "@odata.type": "#microsoft.graph.workbookTable",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "Legacy Id value",
  "name": "Name value",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "Style value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooktable"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookTable",
  "id": "22dfbd4d-bd4d-22df-4dbd-df224dbddf22",
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "legacyId": "Legacy Id value",
  "name": "Name value",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "Style value"
}
```

