---
title: "Create workbookWorksheetProtection"
description: "Create a new workbookWorksheetProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookWorksheetProtection

Namespace: microsoft.graph

Create a new [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.workbookWorksheetProtection not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

The following table shows the properties that are required when you create the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookworksheetprotectionoptions.md)||
|protected|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookworksheetprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookWorksheetProtection not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookworksheetprotection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "id": "2694d3f1-d3f1-2694-f1d3-9426f1d39426",
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

