---
title: "Create importedAppleDeviceIdentity"
description: "Create a new importedAppleDeviceIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create importedAppleDeviceIdentity

Namespace: microsoft.graph

Create a new [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|serialNumber|String|Device serial number|
|requestedEnrollmentProfileId|String|Enrollment profile Id admin intends to apply to the device during next enrollment|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|The time enrollment profile was assigned to the device|
|isSupervised|Boolean|Indicates if the Apple device is supervised. More information is at: https://support.apple.com/en-us/HT202837|
|discoverySource|Enumeration|Apple device discovery source. Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Indicates if the device is deleted from Apple Business Manager|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|description|String|The description of the device|
|enrollmentState|Enumeration|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response
If successful, this method returns a `201 Created` response code and a [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_importedappledeviceidentity_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 515

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:19.9727635+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
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
  "@odata.type": "microsoft.graph.importedappledeviceidentity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "84ec82a3-82a3-84ec-a382-ec84a382ec84",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:19.9727635+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastContactedDateTime": "2016-12-31T23:59:02.6652919+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

