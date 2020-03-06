---
title: "Add importedDeviceIdentities"
description: "Add importedDeviceIdentities by posting to the importedDeviceIdentities collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add importedDeviceIdentities

Namespace: microsoft.graph

Add importedDeviceIdentities by posting to the importedDeviceIdentities collection.

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
POST /deviceManagement/importedDeviceIdentities/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/importeddeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|Imported Device Identifier|
|importedDeviceIdentityType|Enumeration|Type of Imported Device Identity. Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|description|String|The description of the device|
|enrollmentState|Enumeration|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response
If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/importeddeviceidentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_importeddeviceidentity_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "2017-01-01T00:03:00.599191+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importeddeviceidentity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 506

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "c4910543-0543-c491-4305-91c4430591c4",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastContactedDateTime": "2017-01-01T00:03:00.599191+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

