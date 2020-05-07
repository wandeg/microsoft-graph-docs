---
title: "Create importedAppleDeviceIdentities"
description: "Create a new importedAppleDeviceIdentities object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create importedAppleDeviceIdentities

Namespace: microsoft.graph

Create a new importedAppleDeviceIdentities object.

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.

The following table shows the properties that are required when you create the [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|serialNumber|String|**TODO: Add Description**|
|requestedEnrollmentProfileId|String|**TODO: Add Description**|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|**TODO: Add Description**|
|isSupervised|Boolean|**TODO: Add Description**|
|discoverySource|discoverySource|**TODO: Add Description**. Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastContactedDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|platform|**TODO: Add Description**. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response

If successful, this method returns a `201 Created` response code and an [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_importedappledeviceidentity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-Type: application/json
Content-length: 440

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": "Boolean",
  "discoverySource": "String",
  "isDeleted": "Boolean",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedappledeviceidentity"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "2e3eabdb-abdb-2e3e-dbab-3e2edbab3e2e",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": "Boolean",
  "discoverySource": "String",
  "isDeleted": "Boolean",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```

