---
title: "getEffectiveDeviceEnrollmentConfigurations"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getEffectiveDeviceEnrollmentConfigurations

Namespace: microsoft.graph



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
GET /me/getEffectiveDeviceEnrollmentConfigurations
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
GET /me/managedDevices/{managedDeviceId}/users/{userId}/getEffectiveDeviceEnrollmentConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_geteffectivedeviceenrollmentconfigurations"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getEffectiveDeviceEnrollmentConfigurations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceenrollmentconfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "63d9d882-d882-63d9-82d8-d96382d8d963",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
      "version": 7
    }
  ]
}
```

