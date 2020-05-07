---
title: "importedAppleDeviceIdentity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedAppleDeviceIdentity resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[importAppleDeviceIdentityList](../api/importedappledeviceidentity-importappledeviceidentitylist.md)|[importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) collection|**TODO: Add Description**|
|[List importedAppleDeviceIdentities](../api/deponboardingsetting-list-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) collection|Get the importedAppleDeviceIdentities from the importedAppleDeviceIdentities navigation property.|
|[Create importedAppleDeviceIdentities](../api/deponboardingsetting-post-importedappledeviceidentities.md)|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md)|Create a new importedAppleDeviceIdentities object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoverySource|discoverySource|**TODO: Add Description**. Possible values are: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|**TODO: Add Description**|
|isSupervised|Boolean|**TODO: Add Description**|
|lastContactedDateTime|DateTimeOffset|**TODO: Add Description**|
|platform|platform|**TODO: Add Description**. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|**TODO: Add Description**|
|requestedEnrollmentProfileId|String|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

