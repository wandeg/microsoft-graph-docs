---
title: "importedAppleDeviceIdentity resource type"
description: "The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device ."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedAppleDeviceIdentity resource type


Namespace: microsoft.graph

The importedAppleDeviceIdentity resource represents the imported device identity of an Apple device .


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get importedAppleDeviceIdentity](../api/importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Read the properties and relationships of an [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.|
|[Update importedAppleDeviceIdentity](../api/importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Update the properties of an [importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) object.|
|[importAppleDeviceIdentityList](../api/importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|description|String|The description of the device|
|discoverySource|discoverySource|Apple device discovery source. Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|enrollmentState|enrollmentState|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|Indicates if the device is deleted from Apple Business Manager|
|isSupervised|Boolean|Indicates if the Apple device is supervised. More information is at: https://support.apple.com/en-us/HT202837|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|platform|platform|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|The time enrollment profile was assigned to the device|
|requestedEnrollmentProfileId|String|Enrollment profile Id admin intends to apply to the device during next enrollment|
|serialNumber|String|Device serial number|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
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
  "platform": "String"
}
```

