---
title: "List securityBaselineSettingStates"
description: "List properties and relationships of the securityBaselineSettingState objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List securityBaselineSettingStates

Namespace: microsoft.graph

List properties and relationships of the [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) objects.

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
GET /me/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_securitybaselinesettingstate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.securitybaselinesettingstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineSettingState",
      "id": "a84fce29-ce29-a84f-29ce-4fa829ce4fa8",
      "settingName": "Setting Name value",
      "state": "String",
      "settingCategoryId": "Setting Category Id value"
    }
  ]
}
```

