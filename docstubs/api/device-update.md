---
title: "Update device"
description: "Update the properties of a device object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update device

Namespace: microsoft.graph

Update the properties of a [device](../resources/device.md) object.

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
PATCH /devices/{devicesId}
PATCH /me/devices/{deviceId}
PATCH /users/{usersId}/devices/{deviceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [device](../resources/device.md) object.

The following table shows the properties that are required when you create the [device](../resources/device.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|accountEnabled|Boolean||
|alternativeSecurityIds|[alternativeSecurityId](../resources/alternativesecurityid.md) collection||
|approximateLastSignInDateTime|DateTimeOffset||
|complianceExpirationDateTime|DateTimeOffset||
|deviceId|String||
|deviceMetadata|String||
|deviceVersion|Int32||
|displayName|String||
|isCompliant|Boolean||
|isManaged|Boolean||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesSyncEnabled|Boolean||
|operatingSystem|String||
|operatingSystemVersion|String||
|physicalIds|String collection||
|profileType|String||
|systemLabels|String collection||
|trustType|String||
|Name|String||
|Manufacturer|String||
|Model|String||
|Kind|String||
|Status|String||
|Platform|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [device](../resources/device.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_device"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/devices/{devicesId}
Content-type: application/json
Content-length: 1253

{
  "@odata.type": "#microsoft.graph.device",
  "deletedDateTime": "2016-12-31T23:58:50.3020202+00:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2016-12-31T23:57:38.2492135+00:00",
  "complianceExpirationDateTime": "2016-12-31T23:58:37.1990152+00:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:00:59.4441492+00:00",
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
Content-Length: 1302

{
  "@odata.type": "#microsoft.graph.device",
  "id": "32360279-0279-3236-7902-363279023632",
  "deletedDateTime": "2016-12-31T23:58:50.3020202+00:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2016-12-31T23:57:38.2492135+00:00",
  "complianceExpirationDateTime": "2016-12-31T23:58:37.1990152+00:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:00:59.4441492+00:00",
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
```

