---
title: "List deviceManagementSettingCategories"
description: "List properties and relationships of the deviceManagementSettingCategory objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementSettingCategories

Namespace: microsoft.graph

List properties and relationships of the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) objects.

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
GET /deviceManagement/categories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementsettingcategory"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/categories
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementsettingcategory)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
      "id": "fcc4bc02-bc02-fcc4-02bc-c4fc02bcc4fc",
      "displayName": "Display Name value"
    }
  ]
}
```

