---
title: "List devices"
description: "Get the devices from the devices navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List devices

Namespace: microsoft.graph

Get the devices from the devices navigation property.

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
GET /me/devices
GET /users/{usersId}/devices
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [device](../resources/device.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/devices
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.device)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.device",
      "id": "83570c14-0c14-8357-140c-5783140c5783",
      "deletedDateTime": "2017-01-01T00:00:54.363956+03:00",
      "accountEnabled": true,
      "alternativeSecurityIds": [
        {
          "@odata.type": "microsoft.graph.alternativeSecurityId",
          "type": 4,
          "identityProvider": "Identity Provider value",
          "key": "a2V5"
        }
      ],
      "approximateLastSignInDateTime": "2017-01-01T00:03:29.7452379+03:00",
      "complianceExpirationDateTime": "2017-01-01T00:01:14.0335247+03:00",
      "deviceId": "Device Id value",
      "deviceMetadata": "Device Metadata value",
      "deviceVersion": 13,
      "displayName": "Display Name value",
      "isCompliant": true,
      "isManaged": true,
      "onPremisesLastSyncDateTime": "2016-12-31T23:57:03.0856135+03:00",
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
      "trustType": "Trust Type value",
      "Name": "Name value",
      "Manufacturer": "Manufacturer value",
      "Model": "Model value",
      "Kind": "Kind value",
      "Status": "Status value",
      "Platform": "Platform value"
    }
  ]
}
```

