---
title: "importedDeviceIdentity resource type"
description: "The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedDeviceIdentity resource type


Namespace: microsoft.graph

The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get importedDeviceIdentity](../api/importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Read properties and relationships of the [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[Update importedDeviceIdentity](../api/importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md)|Update the properties of a [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.|
|[importDeviceIdentityList](../api/importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection||
|[searchExistingIdentities](../api/importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|description|String|The description of the device|
|enrollmentState|Enumeration|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|Imported Device Identifier|
|importedDeviceIdentityType|Enumeration|Type of Imported Device Identity. Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|platform|Enumeration|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```

