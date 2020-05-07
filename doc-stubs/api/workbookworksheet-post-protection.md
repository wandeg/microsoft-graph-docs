---
title: "Create protection"
description: "Create a new protection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create protection

Namespace: microsoft.graph

Create a new protection object.

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
POST /workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/protection
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object.

The following table shows the properties that are required when you create the [workbookWorksheetProtection](../resources/workbookworksheetprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|options|[workbookWorksheetProtectionOptions](../resources/workbookworksheetprotectionoptions.md)|**TODO: Add Description**|
|protected|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [workbookWorksheetProtection](../resources/workbookworksheetprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookworksheetprotection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/workbook/names/{workbookNamedItemId}/worksheet/protection
Content-Type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
  },
  "protected": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookworksheetprotection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookWorksheetProtection",
  "id": "e87b7789-7789-e87b-8977-7be889777be8",
  "options": {
    "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
  },
  "protected": "Boolean"
}
```

