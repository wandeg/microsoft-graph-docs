---
title: "importedDeviceIdentityResult resource type"
description: "The importedDeviceIdentityResult resource represents the result of attempting to import a device identity."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedDeviceIdentityResult resource type


Namespace: microsoft.graph

The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.


Inherits from [importedDeviceIdentity](../resources/importeddeviceidentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List importedDeviceIdentityResults](../api/importeddeviceidentityresult-list.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection|List properties and relationships of the [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) objects.|
|[Get importedDeviceIdentityResult](../api/importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md)|Read properties and relationships of the [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.|
|[Create importedDeviceIdentityResult](../api/importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md)|Create a new [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.|
|[Delete importedDeviceIdentityResult](../api/importeddeviceidentityresult-delete.md)|None|Deletes a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md).|
|[Update importedDeviceIdentityResult](../api/importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md)|Update the properties of a [importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|description|String|The description of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|enrollmentState|Enumeration|The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|importedDeviceIdentityType|Enumeration|Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md)|
|platform|Enumeration|The platform of the Device. Inherited from [importedDeviceIdentity](../resources/importeddeviceidentity.md). Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status of imported device identity|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult",
  "baseType": "microsoft.graph.importedDeviceIdentity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```

