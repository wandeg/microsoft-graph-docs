---
title: "Update importedAppleDeviceIdentity"
description: "Update the properties of a importedAppleDeviceIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update importedAppleDeviceIdentity

Namespace: microsoft.graph

Update the properties of a [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|serialNumber|String||
|requestedEnrollmentProfileId|String||
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset||
|isSupervised|Boolean||
|discoverySource|Enumeration| Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean||
|createdDateTime|DateTimeOffset||
|lastContactedDateTime|DateTimeOffset||
|description|String||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|Enumeration| Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_importedappledeviceidentity"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/{importedAppleDeviceIdentityId}
Content-type: application/json
Content-length: 515

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2016-12-31T23:59:00.8885497+00:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "lastContactedDateTime": "2017-01-01T00:03:12.8627535+00:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
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
Content-Length: 623

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "1a964b17-4b17-1a96-174b-961a174b961a",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2016-12-31T23:59:00.8885497+00:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
  "lastContactedDateTime": "2017-01-01T00:03:12.8627535+00:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

