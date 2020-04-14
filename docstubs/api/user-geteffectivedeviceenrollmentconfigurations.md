---
title: "user: getEffectiveDeviceEnrollmentConfigurations"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_geteffectivedeviceenrollmentconfigurations"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/getEffectiveDeviceEnrollmentConfigurations
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "ccb26467-6467-ccb2-6764-b2cc6764b2cc",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2016-12-31T23:56:44.6706005+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:31.4610409+03:00",
      "version": 7
    }
  ]
}
```

