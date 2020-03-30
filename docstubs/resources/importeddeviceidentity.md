---
title: "importedDeviceIdentity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedDeviceIdentity resource type


Namespace: microsoft.graph




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
|createdDateTime|DateTimeOffset||
|description|String||
|enrollmentState|Enumeration| Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String||
|importedDeviceIdentityType|Enumeration| Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|platform|Enumeration| Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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

