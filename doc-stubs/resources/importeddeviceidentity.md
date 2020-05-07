---
title: "importedDeviceIdentity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedDeviceIdentity resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[importDeviceIdentityList](../api/importeddeviceidentity-importdeviceidentitylist.md)|[importedDeviceIdentityResult](../resources/importeddeviceidentityresult.md) collection|**TODO: Add Description**|
|[searchExistingIdentities](../api/importeddeviceidentity-searchexistingidentities.md)|[importedDeviceIdentity](../resources/importeddeviceidentity.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|enrollmentState|enrollmentState|**TODO: Add Description**. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|importedDeviceIdentifier|String|**TODO: Add Description**|
|importedDeviceIdentityType|importedDeviceIdentityType|**TODO: Add Description**. Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|platform|platform|**TODO: Add Description**. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

