---
title: "Create device"
description: "Create a new device object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create device

Namespace: microsoft.graph

Create a new [device](../resources/device.md) object.

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
POST /devices
POST /me/devices
POST /users/{usersId}/devices
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [device](../resources/device.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}
-->
``` http
POST https://graph.microsoft.com/localtest/devices
Content-type: application/json
Content-length: 1253

{
  "@odata.type": "#microsoft.graph.device",
  "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2016-12-31T23:59:02.5499427+03:00",
  "complianceExpirationDateTime": "2017-01-01T00:03:17.1122794+03:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2016-12-31T23:58:26.0302388+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1302

{
  "@odata.type": "#microsoft.graph.device",
  "id": "398d4484-4484-398d-8444-8d3984448d39",
  "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "microsoft.graph.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2016-12-31T23:59:02.5499427+03:00",
  "complianceExpirationDateTime": "2017-01-01T00:03:17.1122794+03:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2016-12-31T23:58:26.0302388+03:00",
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

