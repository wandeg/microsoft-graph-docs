---
title: "Update importedDeviceIdentityResult"
description: "Update the properties of a importedDeviceIdentityResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update importedDeviceIdentityResult

Namespace: microsoft.graph

Update the properties of a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.

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
PATCH ** Entity URI for microsoft.graph.importedDeviceIdentityResult not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.

The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|importedDeviceIdentityType|Enumeration|Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|description|String|The description of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|enrollmentState|Enumeration|The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration|The platform of the Device. Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status of imported device identity|



## Response
If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_importeddeviceidentityresult"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.importedDeviceIdentityResult not found
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
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
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "5a6ef58f-f58f-5a6e-8ff5-6e5a8ff56e5a",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```

