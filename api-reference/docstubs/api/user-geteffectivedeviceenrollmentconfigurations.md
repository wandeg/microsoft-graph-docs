---
title: "user: getEffectiveDeviceEnrollmentConfigurations"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# getEffectiveDeviceEnrollmentConfigurations

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/getEffectiveDeviceEnrollmentConfigurations
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
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
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "7f6f5272-5272-7f6f-7252-6f7f72526f7f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2016-12-31T23:57:35.7108579+03:00",
      "lastModifiedDateTime": "2016-12-31T23:58:38.9820934+03:00",
      "version": 7
    }
  ]
}
```

