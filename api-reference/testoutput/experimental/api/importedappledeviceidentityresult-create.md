---
title: "Create importedAppleDeviceIdentityResult"
description: "Create a new importedAppleDeviceIdentityResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create importedAppleDeviceIdentityResult

Create a new [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object.

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
POST ** Collection URI for microsoft.graph.importedAppleDeviceIdentityResult not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the importedAppleDeviceIdentityResult object.

The following table shows the properties that are required when you create the importedAppleDeviceIdentityResult.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|serialNumber|String|Device serial number Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|requestedEnrollmentProfileId|String|Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|isSupervised|Boolean|Indicates if the Apple device is supervised. More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|discoverySource|Enumeration|Apple device discovery source. Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md). Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|createdDateTime|DateTimeOffset|Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|description|String|The description of the device Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md)|
|enrollmentState|Enumeration|The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md). Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration|The platform of the Device. Inherited from [importedAppleDeviceIdentity](../resources/importedAppleDeviceIdentity.md). Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status of imported device identity|



## Response
If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_importedappledeviceidentityresult_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.importedAppleDeviceIdentityResult not found
Content-type: application/json
Content-length: 540

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:00:11.9968518+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
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
  "@odata.type": "microsoft.graph.importedappledeviceidentityresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 648

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "a0706119-6119-a070-1961-70a0196170a0",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:00:11.9968518+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastContactedDateTime": "2016-12-31T23:57:05.6212876+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```

