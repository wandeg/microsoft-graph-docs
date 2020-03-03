---
title: "Create importedDeviceIdentityResult"
description: "Create a new importedDeviceIdentityResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create importedDeviceIdentityResult

Create a new [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.

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
POST ** Collection URI for microsoft.graph.importedDeviceIdentityResult not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the importedDeviceIdentityResult object.

The following table shows the properties that are required when you create the importedDeviceIdentityResult.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md)|
|importedDeviceIdentityType|Enumeration|Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md). Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md)|
|createdDateTime|DateTimeOffset|Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md)|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md)|
|description|String|The description of the device Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md)|
|enrollmentState|Enumeration|The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md). Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration|The platform of the Device. Inherited from [importedDeviceIdentity](../resources/importedDeviceIdentity.md). Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status of imported device identity|



## Response
If successful, this method returns a `201 Created` response code and a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_importeddeviceidentityresult_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.importedDeviceIdentityResult not found
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "2016-12-31T23:57:05.6212876+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.importeddeviceidentityresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 532

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "1f624535-4535-1f62-3545-621f3545621f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastContactedDateTime": "2016-12-31T23:57:05.6212876+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```

