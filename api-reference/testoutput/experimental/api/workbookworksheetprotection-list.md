---
title: "List workbookWorksheetProtections"
description: "List properties and relationships of the workbookWorksheetProtection objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookWorksheetProtections

List properties and relationships of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookWorksheetProtection not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookworksheetprotection"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.workbookWorksheetProtection not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookworksheetprotection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 677

{
  "value": [
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
  ]
}
```

