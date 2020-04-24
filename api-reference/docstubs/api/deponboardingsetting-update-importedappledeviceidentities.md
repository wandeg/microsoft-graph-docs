---
title: "Update importedAppleDeviceIdentities"
description: "Update the properties of an importedAppleDeviceIdentities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update importedAppleDeviceIdentities

Namespace: microsoft.graph

Update the properties of an importedAppleDeviceIdentities object.

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
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|serialNumber|String|Device serial number|
|requestedEnrollmentProfileId|String|Enrollment profile Id admin intends to apply to the device during next enrollment|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|The time enrollment profile was assigned to the device|
|isSupervised|Boolean|Indicates if the Apple device is supervised. More information is at: https://support.apple.com/en-us/HT202837|
|discoverySource|discoverySource|Apple device discovery source. Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Indicates if the device is deleted from Apple Business Manager|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|description|String|The description of the device|
|enrollmentState|enrollmentState|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|platform|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_importedappledeviceidentities"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-Type: application/json
Content-length: 515

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2016-12-31T23:57:22.1659668+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "lastContactedDateTime": "2017-01-01T00:00:56.6420947+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "15330b01-0b01-1533-010b-3315010b3315",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2016-12-31T23:57:22.1659668+03:00",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastContactedDateTime": "2017-01-01T00:00:56.6420947+03:00",
  "description": "Description value",
  "enrollmentState": "String",
  "platform": "String"
}
```

