---
title: "importedAppleDeviceIdentityResult resource type"
description: "The importedAppleDeviceIdentityResult resource represents the result of attempting to import Apple devices identities."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedAppleDeviceIdentityResult resource type


Namespace: microsoft.graph

The importedAppleDeviceIdentityResult resource represents the result of attempting to import Apple devices identities.


Inherits from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List importedAppleDeviceIdentityResults](../api/importedappledeviceidentityresult-list.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) collection|List properties and relationships of the [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) objects.|
|[Get importedAppleDeviceIdentityResult](../api/importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md)|Read properties and relationships of the [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object.|
|[Create importedAppleDeviceIdentityResult](../api/importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md)|Create a new [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object.|
|[Delete importedAppleDeviceIdentityResult](../api/importedappledeviceidentityresult-delete.md)|None|Deletes a [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md).|
|[Update importedAppleDeviceIdentityResult](../api/importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md)|Update the properties of a [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|description|String|The description of the device Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|discoverySource|Enumeration|Apple device discovery source. Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md). Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|enrollmentState|Enumeration|The state of the device in Intune Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md). Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|Indicates if the device is deleted from Apple Business Manager Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|isSupervised|Boolean|Indicates if the Apple device is supervised. More information is at: https://support.apple.com/en-us/HT202837 Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|platform|Enumeration|The platform of the Device. Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md). Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|The time enrollment profile was assigned to the device Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|String|Enrollment profile Id admin intends to apply to the device during next enrollment Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|serialNumber|String|Device serial number Inherited from [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|
|status|Boolean|Status of imported device identity|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult",
  "baseType": "microsoft.graph.importedAppleDeviceIdentity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```

