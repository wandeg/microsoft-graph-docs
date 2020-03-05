---
title: "List iosManagedAppRegistrations"
description: "List properties and relationships of the iosManagedAppRegistration objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List iosManagedAppRegistrations

Namespace: microsoft.graph

List properties and relationships of the [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) objects.

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
GET ** Collection URI for microsoft.graph.iosManagedAppRegistration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/iosmanagedappregistration.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_iosmanagedappregistration"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.iosManagedAppRegistration not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.iosmanagedappregistration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 802

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
      "id": "96cd9296-9296-96cd-9692-cd969692cd96",
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "lastSyncDateTime": "2016-12-31T23:59:45.269987+03:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "String"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "version": "Version value"
    }
  ]
}
```

