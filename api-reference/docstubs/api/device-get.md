---
title: "Get device"
description: "Read properties and relationships of a device object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get device

Namespace: microsoft.graph

Read properties and relationships of a [device](../resources/device.md) object.

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
GET /devices/{devicesId}
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
If successful, this method returns a `200 OK` response code and a [device](../resources/device.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_device"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{devicesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.device",
    "id": "0fa3c37f-c37f-0fa3-7fc3-a30f7fc3a30f",
    "deletedDateTime": "2016-12-31T23:59:39.086137+00:00",
    "accountEnabled": true,
    "alternativeSecurityIds": [
      {
        "@odata.type": "microsoft.graph.alternativeSecurityId",
        "type": 4,
        "identityProvider": "Identity Provider value",
        "key": "a2V5"
      }
    ],
    "approximateLastSignInDateTime": "2017-01-01T00:01:23.7320263+00:00",
    "complianceExpirationDateTime": "2016-12-31T23:58:11.1367117+00:00",
    "deviceId": "Device Id value",
    "deviceMetadata": "Device Metadata value",
    "deviceVersion": 13,
    "displayName": "Display Name value",
    "isCompliant": true,
    "isManaged": true,
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:21.5753431+00:00",
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
}
```

