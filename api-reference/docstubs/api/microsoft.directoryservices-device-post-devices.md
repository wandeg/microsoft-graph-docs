---
title: "Create device"
description: "Create a new device object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create device

Namespace: Microsoft.DirectoryServices

Create a new [device](../resources/microsoft.directoryservices-device.md) object.

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
POST /devices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [device](../resources/microsoft.directoryservices-device.md) object.

The following table shows the properties that are required when you create the [device](../resources/microsoft.directoryservices-device.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|accountEnabled|Boolean|**TODO: Add Description**|
|alternativeSecurityIds|[alternativeSecurityId](../resources/microsoft.directoryservices-alternativesecurityid.md) collection|**TODO: Add Description**|
|approximateLastSignInDateTime|DateTimeOffset|**TODO: Add Description**|
|complianceExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|deviceMetadata|String|**TODO: Add Description**|
|deviceVersion|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isCompliant|Boolean|**TODO: Add Description**|
|isManaged|Boolean|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|operatingSystem|String|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|
|physicalIds|String collection|**TODO: Add Description**|
|profileType|String|**TODO: Add Description**|
|systemLabels|String collection|**TODO: Add Description**|
|trustType|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [device](../resources/microsoft.directoryservices-device.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}
-->
``` http
POST https://graph.microsoft.com/changelog/devices
Content-Type: application/json
Content-length: 1097

{
  "@odata.type": "#Microsoft.DirectoryServices.device",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "Microsoft.DirectoryServices.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2017-01-01T00:02:10.3629339+00:00",
  "complianceExpirationDateTime": "2017-01-01T00:00:23.7887185+00:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.device"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.device",
  "id": "af73946f-946f-af73-6f94-73af6f9473af",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "accountEnabled": true,
  "alternativeSecurityIds": [
    {
      "@odata.type": "Microsoft.DirectoryServices.alternativeSecurityId",
      "type": 4,
      "identityProvider": "Identity Provider value",
      "key": "a2V5"
    }
  ],
  "approximateLastSignInDateTime": "2017-01-01T00:02:10.3629339+00:00",
  "complianceExpirationDateTime": "2017-01-01T00:00:23.7887185+00:00",
  "deviceId": "Device Id value",
  "deviceMetadata": "Device Metadata value",
  "deviceVersion": 13,
  "displayName": "Display Name value",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
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
```

