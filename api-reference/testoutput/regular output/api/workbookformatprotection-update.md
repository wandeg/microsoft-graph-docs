---
title: "Update workbookFormatProtection"
description: "Update the properties of a workbookFormatProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookFormatProtection

Update the properties of a [workbookFormatProtection](../resources/workbookformatprotection.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookFormatProtection not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookFormatProtection](../resources/workbookFormatProtection.md) object.

The following table shows the properties that are required when you create the [workbookFormatProtection](../resources/workbookformatprotection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|formulaHidden|Boolean||
|locked|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookFormatProtection](../resources/workbookformatprotection.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookformatprotection"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.workbookFormatProtection not found
Content-type: application/json
Content-length: 111

{
  "@odata.type": "#microsoft.graph.workbookFormatProtection",
  "formulaHidden": true,
  "locked": true
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
Content-Length: 160

{
  "@odata.type": "#microsoft.graph.workbookFormatProtection",
  "id": "eebb12c4-12c4-eebb-c412-bbeec412bbee",
  "formulaHidden": true,
  "locked": true
}
```

