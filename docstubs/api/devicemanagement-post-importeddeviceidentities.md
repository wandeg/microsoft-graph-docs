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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedDeviceIdentity](../resources/importeddeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String||
|importedDeviceIdentityType|Enumeration| Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset||
|createdDateTime|DateTimeOffset||
|lastContactedDateTime|DateTimeOffset||
|description|String||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration| Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



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
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "2017-01-01T00:00:27.4696173+00:00",
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
Content-Length: 507

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "d450c1e2-c1e2-d450-e2c1-50d4e2c150d4",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "lastContactedDateTime": "2017-01-01T00:00:27.4696173+00:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

