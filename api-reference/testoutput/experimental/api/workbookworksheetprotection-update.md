---
title: "Update workbookWorksheetProtection"
description: "Update the properties of a workbookWorksheetProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookWorksheetProtection

Update the properties of a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/protection
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookWorksheetProtection](../resources/workbookWorksheetProtection.md) object.

The following table shows the properties that are required when you create the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookWorksheetProtectionOptions.md)||
|protected|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookworksheetprotection"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/protection
Content-type: application/json
Content-length: 527

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "id": "eea3f130-f130-eea3-30f1-a3ee30f1a3ee",
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
```

