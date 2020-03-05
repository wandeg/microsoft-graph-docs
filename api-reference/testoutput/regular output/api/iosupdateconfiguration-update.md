---
title: "Update iosUpdateConfiguration"
description: "Update the properties of a iosUpdateConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update iosUpdateConfiguration

Namespace: microsoft.graph

Update the properties of a [iosUpdateConfiguration](../resources/iosupdateconfiguration.md) object.

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
PATCH ** Entity URI for microsoft.graph.iosUpdateConfiguration not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/iosupdateconfiguration.md) object.

The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/iosupdateconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|activeHoursStart|TimeOfDay|Active Hours Start (active hours mean the time window when updates install should not happen)|
|activeHoursEnd|TimeOfDay|Active Hours End (active hours mean the time window when updates install should not happen)|
|scheduledInstallDays|Enumeration collection|Days in week for which active hours are configured. This collection can contain a maximum of 7 elements. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|utcTimeOffsetInMinutes|Int32|UTC Time Offset indicated in minutes|



## Response
If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/iosupdateconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_iosupdateconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.iosUpdateConfiguration not found
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:35.0320000",
  "activeHoursEnd": "11:59:54.5850000",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 6
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
Content-Length: 495

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "1359b4dc-b4dc-1359-dcb4-5913dcb45913",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:35.0320000",
  "activeHoursEnd": "11:59:54.5850000",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

