---
title: "List devices"
description: "List properties and relationships of the device objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List devices

Namespace: microsoft.graph

List properties and relationships of the [device](../resources/device.md) objects.

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
GET /devices
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [device](../resources/device.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/localtest/devices
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.device)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1321

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.device",
      "id": "cbd2d7c2-d7c2-cbd2-c2d7-d2cbc2d7d2cb",
      "deletedDateTime": "2017-01-01T00:02:06.0464622+03:00",
      "accountEnabled": true,
      "alternativeSecurityIds": [
        {
          "@odata.type": "microsoft.graph.alternativeSecurityId",
          "type": 4,
          "identityProvider": "Identity Provider value",
          "key": "a2V5"
        }
      ],
      "approximateLastSignInDateTime": "2016-12-31T23:58:50.577268+03:00",
      "complianceExpirationDateTime": "2017-01-01T00:01:46.0720276+03:00",
      "deviceId": "Device Id value",
      "deviceMetadata": "Device Metadata value",
      "deviceVersion": 13,
      "displayName": "Display Name value",
      "isCompliant": true,
      "isManaged": true,
      "mdmAppId": "Mdm App Id value",
      "onPremisesLastSyncDateTime": "2017-01-01T00:00:16.9182164+03:00",
      "onPremisesSyncEnabled": true,
      "operatingSystem": "Operating System value",
      "operatingSystemVersion": "Operating System Version value",
      "physicalIds": [
        "Physical Ids value"
      ],
      "profileType": "Profile Type value",
      "systemLabels": [
        "System Labels value"
      ],
      "trustType": "Trust Type value"
    }
  ]
}
```

