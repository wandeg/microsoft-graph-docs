---
title: "List protection"
description: "Get the workbookWorksheetProtections from the protection navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List protection

Namespace: microsoft.graph

Get the workbookWorksheetProtections from the protection navigation property.

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
GET /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/protection
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/protection
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookworksheetprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
      "id": "33c63a6d-3a6d-33c6-6d3a-c6336d3ac633",
      "options": {
        "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions",
        "allowAutoFilter": true,
        "allowDeleteColumns": true,
        "allowDeleteRows": true,
        "allowFormatCells": true,
        "allowFormatColumns": true,
        "allowFormatRows": true,
        "allowInsertColumns": true,
        "allowInsertHyperlinks": true,
        "allowInsertRows": true,
        "allowPivotTables": true,
        "allowSort": true
      },
      "protected": true
    }
  ]
}
```

